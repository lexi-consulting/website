<script>
    let ratio = 206;
    export let radius = 540;
    export let stroke = radius*(ratio/540);
</script>
<g transform="matrix(1.83 0 0 1.83 {radius} {radius})">
    <path
        class="fill-valiant quarter"
        vector-effect="non-scaling-stroke"
        d="M 0 0 L 0 {stroke} A {stroke} {stroke} 0 0 1 -{stroke} 0 L 0 0 Z"
        stroke-linecap="round" />
</g>