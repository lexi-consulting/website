<script lang="ts">
	import Text from "./Text.svelte";
	import Boundary from "./Boundary.svelte";
	import SVG from "$lib/img/SVG.svelte";
	import AllQuadrants from "./AllQuadrants.svelte";

	let w;
	let h;
</script>
<div
	class="grid place-items-center h-full w-full"
	bind:clientWidth={w} bind:clientHeight={h}
	>
	<SVG 
		config={{width: w, height: h}} 
		radius={Math.min(w,h)/2} 
		let:radius={radius}
		>
		<AllQuadrants {radius}/>
		<Boundary {radius}/>
		<Text {radius}/>
	</SVG>
</div>