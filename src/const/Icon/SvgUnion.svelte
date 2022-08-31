<script lang="ts">
    export let paths: Array<string>;
    export let width: number;
    export let height: number;
    export let style: string="";
</script>
<svg class="{style}" width={width} height={height} viewBox="0 0 {width} {height}" fill="none" xmlns="http://www.w3.org/2000/svg">
    {#each paths as path}
        <path d={path} fill="currentColor"/>
    {/each}
</svg>