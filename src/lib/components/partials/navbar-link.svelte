<script lang="ts">
	import { base } from '$app/paths';
	import { page } from '$app/state';

	type Attributo = {
		url: string;
		testo: string;
	};

	let a: Attributo = $props();

	const href = $derived(base + a.url);
	const isActive = $derived(href === page.url.pathname);
</script>

<a
	{href}
	class={{
		'text-primary-foreground hover:bg-secondary hover:text-primary-foreground': !isActive,
		'bg-white': isActive
	}}
>
	{a.testo}
</a>
