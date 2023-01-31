<script lang="ts">
    export let radius :number = 540;

    let defaultRadius = 540;
	let largeRatio = 275;
    let stroke = 0.5*radius*(largeRatio/defaultRadius);
</script>
<g transform="matrix(1.83 0 0 1.83 {radius} {radius})">
    <line
        style="stroke-width: 4; stroke: rgb(29,29,27); "
        vector-effect="non-scaling-stroke" x1=0 y1="-{stroke}" x2=0 y2="{stroke}" />
</g>