<script>
    let ratio = 275;
    export let radius = 540;
    export let stroke = radius*(ratio/540);
</script>
<g transform="matrix(1.83 0 0 1.83 {radius} {radius})">
    <path
        class="fill-radiant quarter"
        vector-effect="non-scaling-stroke"
        d="M 0 0 L -{stroke} 0 A {stroke} {stroke} 0 0 1 0 -{stroke} L 0 0 Z"
        stroke-linecap="round" />
</g>