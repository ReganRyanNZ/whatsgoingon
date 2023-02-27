<script>
	import Counter from './Counter.svelte';
	import map from '$lib/images/map.jpeg';
</script>

<svelte:head>
	<title>What's going on?</title>
</svelte:head>

<img src={map} alt=" " class="backdrop"/>
<h1>
  Nathan is a noble goose
</h1>

<style>

	h1 {
		width: 100%;
    color: blue;
    font-size: 40px;
	}

	.backdrop {
		display: block;
		position: absolute;
    z-index: -100;
		width: 100vw;
	}

</style>
