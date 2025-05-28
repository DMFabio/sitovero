<script lang="ts">
	import { base } from '$app/paths';

	type Attributo = {
		url: string;
		testo: string;
	};

	let a: Attributo = $props();
</script>

<a
	href="{base}{a.url}"
	class="bg-primary text-primary-foreground hover:bg-secondary hover:text-primary-foreground"
	>{a.testo}</a
>
