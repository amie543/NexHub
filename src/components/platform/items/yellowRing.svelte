<script lang="ts">
    import Svg from "icon/Svg.svelte";
    const path= "M82.5 0C36.9333 0 0 36.9333 0 82.5C0 128.067 36.9333 165 82.5 165C128.067 165 165 128.067 165 82.5C165 36.9333 128.067 0 82.5 0ZM82.5 132.605C54.8261 132.605 32.3949 110.174 32.3949 82.5C32.3949 54.8261 54.8261 32.3949 82.5 32.3949C110.174 32.3949 132.605 54.8261 132.605 82.5C132.605 110.174 110.174 132.605 82.5 132.605Z";
    export let width= 165;
    export let height= 165;
    export let style: string = "";
</script>
<div class="{style}">
    <Svg width ={width} height={height} path={path}/>

</div>