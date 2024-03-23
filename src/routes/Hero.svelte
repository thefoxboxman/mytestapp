<script>
	import Counter from "./Counter.svelte";

    import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script>


<section class="stack-l-center">
	<h1 class="text-primary-500 fs-primary-heading stack-l-center">
		<span class="welcome">
			<picture>
				<source srcset={welcome} type="image/webp" />
				<img src={welcome_fallback} alt="Welcome" />
			</picture>
		</span>

		to your new<br />SvelteKit app
	</h1>

	<h2 class="fs-secondary-heading text-primary-400">
		try editing <br /> <strong class="fs-500 text-neutral-100">src/routes/+page.svelte</strong>
	</h2>

	
</section>

<style>
	/* section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	} */

	h1 {
		width: 100%;

	}
	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
	</style>