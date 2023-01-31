<script>
    export let config = {
        radius: 540,
        d: "M 0 0 L -275 0 A 275 275 0 0 1 0 -275 L 0 0 Z",
        fill: "radiant"
    };
</script>
<g transform="matrix(1.83 0 0 1.83 {config.radius} {config.radius})">
    <path
        class="fill-{config.fill} quarter"
        vector-effect="non-scaling-stroke"
        d={config.d}
        stroke-linecap="round" />
</g>