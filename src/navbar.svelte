<script>
	import NavButton from "./menuButton.svelte";
</script>

<!--LINKS TO ICONS-->
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Rounded:opsz,wght,FILL,GRAD@48,400,0,0" />
<!--LINKS TO ICONS-->

<nav class="main-navbar">
	<div class="nav-title-cont">
		<span class="nav-title">
			Programmatic
		</span>
	</div>	
	<div class="nav-menu-cont" >
		<NavButton title="Home" iconName="home"/>
		<NavButton title="Computer" iconName="computer"/>
		<NavButton title="Portfolio" iconName="person"/>
		<NavButton title="Contacts" iconName="contacts"/>
		<NavButton login title="Login" iconName="password"/>
	</div>
</nav>


<style>
	
	:root {
		--title-left-bias : 12rem;
		--nav-cont-bg : #f4f4f4;
		--nav-cont-height : 7rem;
		--nav-title-letter-spacing : 8px;
		--nav-title-font-size : 2rem;
		--nav-menu-btn-bg : #dedede;
		--nav-menu-btn-spacing : 1rem;
		--nav-menu-btn-padding : 1em;
	}


	.nav-title {
		font-size : var(--nav-title-font-size);

		font-family: monospace;
		font-weight : bold;
		letter-spacing: var(--nav-title-letter-spacing);
	}

	.main-navbar {
		display : flex;
		flex-direction: row;
		height : var(--nav-cont-height);

		align-items: center;
		justify-content: center;

		background-color: var(--nav-cont-bg);

		margin : 1em;
	} 


	.nav-title-cont {
		flex : 1;
		padding-left: var(--title-left-bias);
	}

	.nav-menu-cont {
		flex : 1;

		height : 100%;
		width: 100%;
	
		flex-direction: row;
		display : flex;
		justify-content: center;

		gap : var(--nav-menu-btn-spacing);
		padding : 10px;
	}
</style>
