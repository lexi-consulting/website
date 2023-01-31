<script>
    export let lx = 90.2/540;
    export let ly = 47.12/540;
    export let ex = 16.89/540;
    export let ey = 47.12/540;
    
    
    let ratio = 206;
    export let radius = 540;
    let radiusRatio = radius/540;
    export let font = radius*150/540;
</script>

<g transform="matrix({1.66*radiusRatio}  0 0 {1.66*radiusRatio} {radius*radiusRatio} {radius})" xmlns="http://www.w3.org/2000/svg" style="">
    <text xml:space="preserve" font-size="{font}" font-weight="100" font-family="Lato-Thin"
        style="stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-dashoffset: 0; stroke-linejoin: miter; stroke-miterlimit: 4; fill: rgb(255,255,255); fill-rule: nonzero; opacity: 1; white-space: pre;">
        <tspan x="-{lx}" y="{ly}">L</tspan>
        <tspan x="{ex}" y="{ey}">E</tspan>
    </text>
</g>