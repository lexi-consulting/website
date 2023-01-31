<script>
	import QuadrantRadiant from "./QuadrantRadiant.svelte";
	import QuadrantRogue from "./QuadrantRogue.svelte";
	import QuadrantTrue from "./QuadrantTrue.svelte";
	import QuadrantValiant from "./QuadrantValiant.svelte";
	import TextLe from "./TextLE.svelte";
	import TextXi from "./TextXI.svelte";
	import Boundary from "./Boundary.svelte";
	import SVG from "$lib/img/SVG.svelte";

	let defaultRadius = 540;
	let largeRatio = 275;
	let smallRatio = 206;
    let lxRatio = 90.2/540;
    let lyRatio = 47.12/540;
    let exRatio = 16.89/540;
    let eyRatio = 47.122/540;
	let xxRatio = 90.2/540;
    let xyRatio = 47.12/540;
    let ixRatio = 16.89/540;
    let iyRatio = 47.12/540;
	let fontRatio = 150/540;

	let w;
	let h;
</script>
<div
	class="grid place-items-center h-full w-full"
	bind:clientWidth={w} bind:clientHeight={h}
	>
	<SVG config={{width: w, height: h}} radius={Math.min(w,h)/2} let:radius={radius} let:config={config}>
		<QuadrantRadiant 
			{radius} 
			stroke={radius*(largeRatio/defaultRadius)/2}/>
		<QuadrantRogue {radius} stroke={radius*(smallRatio/defaultRadius)/2}/>
		<QuadrantValiant {radius} stroke={radius*(smallRatio/defaultRadius)/2}/>
		<QuadrantTrue {radius} stroke={radius*(largeRatio/defaultRadius)/2}/>
		<TextLe 
			{radius} 
			lx={lxRatio*radius}
			ly={lyRatio*radius}
			ex={exRatio*radius}
			ey={eyRatio*radius}
			font={fontRatio*radius}/>
		<TextXi 
			{radius} 
			xx={xxRatio*radius}
			xy={xyRatio*radius}
			ix={ixRatio*radius}
			iy={iyRatio*radius}
			font={fontRatio*radius}/>
		<Boundary {radius} stroke={radius*(largeRatio/defaultRadius)/2}/>
	</SVG>
</div>