<script lang="ts">
    export let path: string;
    export let width: number;
    export let height: number;
    export let strokeWidth: number = 0;
    export let style: string="";
</script>
<svg class="{style}" width={width} height={height} viewBox="0 0 {width} {height}" fill="none" xmlns="http://www.w3.org/2000/svg">
    {#if strokeWidth>0 }
        <path d={path} stroke="currentColor" stroke-width={strokeWidth} stroke-miterlimit="10"/>
    {:else}
        <path d={path} fill="currentColor"/>
    {/if}
</svg>
