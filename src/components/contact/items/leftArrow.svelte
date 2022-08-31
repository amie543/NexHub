<script lang="ts">
    import Svg from "icon/Svg.svelte";
    export let path ="M20 4.16634L14.9713 -0.000325382L14.9713 3.33301L5.36462e-07 3.33301L5.16587e-07 4.99967L14.9713 4.99967L14.9713 8.33301L20 4.16634Z";
    export let width=20;
    export let height=9;
    export let style="";
</script>
<div class="{style} absolute left-4 top-5">
    <Svg width ={width} height={height} path={path}/>

</div>
