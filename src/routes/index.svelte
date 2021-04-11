<script>
	import Marquee from '$lib/Marquee.svelte';

	const banner = ['Lorem', 'ipsum', 'dolor', 'sit', 'amet', 'consectetur', 'adipiscing', 'elit'];
</script>

<main>
	<h1>Hello @keyframe bug!</h1>

	<Marquee>
		{#each banner as word}
			<span style="margin: 0.5rem">{word}</span>
		{/each}
	</Marquee>

	<p>Visit <a class="text-blue-600 underline" href="https://svelte.dev">svelte.dev</a> to learn how to build Svelte apps.</p>
</main>

<style style lang="postcss">
	main {
		@apply text-center;
		@apply p-4;
		@apply mx-auto;
	}

	h1 {
		@apply text-red-600;
		@apply uppercase;
		@apply text-6xl;
		@apply font-thin;
		@apply leading-tight;
		@apply my-16 mx-auto;
		@apply max-w-xs;
	}

	p {
		@apply max-w-xs;
		@apply my-8 mx-auto;
		@apply leading-snug;
	}

	@screen sm {
		h1 {
			@apply max-w-none;
		}

		p {
			@apply max-w-none;
		}
	}
</style>
