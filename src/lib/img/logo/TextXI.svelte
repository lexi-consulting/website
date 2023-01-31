<script>
    export let xx = 90.2/540;
    export let xy = 47.12/540;
    export let ix = 16.89/540;
    export let iy = 47.12/540;
    export let ratio = 206;
    let radiusRatio = 736.11/540;
    export let radius = 540;
    
    export let font = radius*150/540;
</script>

<g transform="matrix(1 0 0 1 {radius*radiusRatio} {radius})" xmlns="http://www.w3.org/2000/svg" style="" >
    <text xml:space="preserve" font-size="{font}" font-weight="100" font-family="Lato-Thin"
        style="stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-dashoffset: 0; stroke-linejoin: miter; stroke-miterlimit: 4; fill: rgb(255,255,255); fill-rule: nonzero; opacity: 1; white-space: pre;">
        <tspan x="-{xx}" y="{xy}">X</tspan>
        <tspan x="{ix}" y="{iy}">I</tspan>
    </text>
</g>