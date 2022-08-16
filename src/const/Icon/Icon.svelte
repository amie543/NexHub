<script lang="ts">
    export let path: string;
    export let size: number;
    export let style: string="";
</script>
<svg width={size} height={size} viewBox="0 0 {size} {size}" class="inline-block {style}" xmlns="http://www.w3.org/2000/svg">
    <path fill="currentColor" d={path}></path>
</svg>
