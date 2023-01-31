<script>
	export let config = {
		width: 540,
		height: 540,
	};
	export let radius = 275;
</script>


<svg
	xmlns="http://www.w3.org/2000/svg" 
	xmlns:xlink="http://www.w3.org/1999/xlink" 
	version="1.1" 
	width={Math.min(config.width,config.height) ?? config.width}
	height={Math.min(config.width,config.height) ??  config.height}
	viewBox="0 0 {Math.min(config.width,config.height) ?? config.width} {Math.min(config.width,config.height) ?? config.height}" 
    class="h-100 w-100 grid place-items-center"
	xml:space="preserve">
	<defs xmlns="http://www.w3.org/2000/svg">
		<style>
			@import url(http://fonts.googleapis.com/css?family=Lato);
		</style>
	</defs>
    <slot {config} {radius}/>
</svg>