<script lang="ts">
    import Svg from 'icon/Svg.svelte';
    const path1="M-47 80.5401L-0.5 107.387L46 80.5401V26.8467L-0.5 0L-47 26.8467V80.5401Z";
    const width1=46; const height1=108;
    const path2="M-47 82.234L-0.5 109.081L46 82.234V28.5406L-0.5 1.69394L-47 28.5406V82.234Z";
    const width2=47; const height2=111;

    export let style: string = "";
</script>
<div class="{style}">
    <Svg path={path1} width={width1} height={height1} style="text-[#FFE031]"/>
    <Svg path={path2} width={width2} height={height2} strokeWidth={2} style="text-[#1D262D] -mt-14"/>
</div>