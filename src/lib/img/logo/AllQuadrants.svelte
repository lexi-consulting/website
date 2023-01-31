<script lang="ts">
	import Quadrant from "./Quadrant.svelte";

    function get_path(lexi :string, ratio :number, radius :number): string{
		let stroke = radius*(ratio/540)/2;
		switch(lexi) { 
			case "radiant": { 
				return `M 0 0 L -${stroke} 0 A ${stroke} ${stroke} 0 0 1 0 -${stroke} L 0 0 Z`;
			} 
			case "rogue": { 
				return `M 0 0 L 0 -${stroke} A ${stroke} ${stroke} 0 0 1 ${stroke} 0 L 0 0 Z`;
			} 
			case "valiant":{
				return `M 0 0 L 0 ${stroke} A ${stroke} ${stroke} 0 0 1 -${stroke} 0 L 0 0 Z`;
			}
			case "true":{
				return `M 0 0 L ${stroke} 0 A ${stroke} ${stroke} 0 0 1 0 ${stroke} L 0 0 Z`;
			}
		} 
		return `M 0 0 L -${stroke} 0 A ${stroke} ${stroke} 0 0 1 0 -${stroke} L 0 0 Z`;
	}

    export let radius :number = 540;
    export let largeRatio :number = 275;
    export let smallRatio :number = 234;

</script>

<g class="logo_quadrants">
    <Quadrant
		config={{
				radius: radius,
				d: get_path("radiant",radius, largeRatio),
				fill: "radiant"
			}}
	/>
	<Quadrant
		config={{
			radius: radius,
			d: get_path("rogue",radius, smallRatio),
			fill: "rogue"
		}}
	/>
	<Quadrant
		config={{
			radius: radius,
			d: get_path("valiant",radius, smallRatio),
			fill: "valiant"
		}}
	/>
	<Quadrant
		config={{
			radius: radius,
			d: get_path("true",radius, largeRatio),
			fill: "true"
		}}
	/>
</g>