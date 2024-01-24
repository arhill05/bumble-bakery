<script>
	export let fullSizeSrc = '';
	export let smallSrc = '';
	export let alt = '';
</script>

<a href={fullSizeSrc} target="_blank">
	<img src={smallSrc} {alt} />
</a>

<style>
	img {
		box-shadow: 8px 9px 0 0 var(--brand-color);
		transition: transform 0.1s ease-in-out;
	}

	img:hover {
		transform: scale(1.05);
		transition: transform 0.1 ease-in-out;
	}
</style>
