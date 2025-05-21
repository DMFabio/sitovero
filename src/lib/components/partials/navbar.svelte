<script>
	import NavbarLink from './navbar-link.svelte';
</script>

<nav class="bg-primary text-primary-foreground flex justify-between">
	<NavbarLink url="/" testo="Home" />

	<div>
		<NavbarLink url="/casabachi" testo="Casa Bachi" />
		<NavbarLink url="/contatti" testo="Contatti" />
		<NavbarLink url="/progetti" testo="Progetti" />
	</div>
</nav>
