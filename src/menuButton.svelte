<script>


	export let title;
	export let iconName;
	export let login = false;

	const handleSubmit = () => {}

	let btnClass = "nav-menu-btn " + (login ? "nav-menu-btn-login" : "");

</script>

<div on:click={handleSubmit} class="{btnClass}">
	<span class="nav-menu-btn-title">
		{title}
	</span>
	<span class="material-symbols-rounded">
		{iconName}
	</span>
</div>

<style>
	:root {
		--nav-btn-letter-spacing : 2px;
		--nav-btn-bg : #2d2d2d;
		--nav-btn-font-size : 1.7em;
		--nav-btn-title-symbol-gap : 4px;
	}
	
	span {
		font-size: var(--nav-btn-font-size);
		font-weight: bold;
		color : white;
	}

	.nav-menu-btn-title {
		font-family: monospace;
		letter-spacing: var(--nav-btn-letter-spacing);
	}

	.nav-menu-btn {
		display : flex;
		flex-direction: row;
		
		align-items: center;
		justify-content: center;
		gap : var(--nav-btn-title-symbol-gap);

		background-color: var(--nav-btn-bg);

		padding : 0em 1.5em;
		border-radius: 10px;


		cursor : pointer;
	}

	.nav-menu-btn-login {
		background-color: #00A300;
	}

</style>
