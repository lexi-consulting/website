<script lang="ts">
    let x : number = 125;
    let y : number = 105.12;
    export let radius :number = 540;
    let radiusRatio :number = radius/540;
    let font :number = radius*150/540;
</script>

<g transform="matrix({radiusRatio}  0 0 {radiusRatio} 463.5 463.5)" xmlns="http://www.w3.org/2000/svg" style="">
    <text xml:space="preserve" font-size="{font}" font-weight="100" font-family="Lato-Thin"
        style="stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-dashoffset: 0; stroke-linejoin: miter; stroke-miterlimit: 4; fill: rgb(255,255,255); fill-rule: nonzero; opacity: 1; white-space: pre;">
        <tspan x="-{x*radiusRatio}" y="{y*radiusRatio}">L E X I</tspan>
    </text>
</g>