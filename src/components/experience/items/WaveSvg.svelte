<script lang="ts">
    import Svg from "icon/Svg.svelte";
    const wavePath = "M2 4L15.83 20.34L29.66 4L43.49 20.34L57.32 4L71.16 20.34L85 4";
    const waveWidth = 87; const waveHeight=24; 
    export let style: string = "";
</script>
<div class="{style}">
    <div class="flex flex-row">
        <Svg width={waveWidth} height={waveHeight} path={wavePath} strokeWidth={4}/>
        <Svg width={waveWidth} height={waveHeight} path={wavePath} strokeWidth={4} style="-ml-1.5"/>
    </div>
    <div class="flex flex-row">
        <Svg width={waveWidth} height={waveHeight} path={wavePath} strokeWidth={4}/>
        <Svg width={waveWidth} height={waveHeight} path={wavePath} strokeWidth={4} style="-ml-1.5"/>
    </div>
</div>