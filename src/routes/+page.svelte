<script>
	import Counter from './Counter.svelte';
	import map from '$lib/images/map.jpeg';
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<section>
	<h1>
		<span class="welcome">
			<picture>
				<img src={map} alt="Map" />
			</picture>
		</span>

		Nathan is a noble goose
	</h1>

	<Counter />
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

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
