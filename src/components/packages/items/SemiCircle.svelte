<script lang="ts">
    import Svg from 'icon/Svg.svelte';
    const path1="M44.0724 0.882774C20.1235 0.750099 0.608397 20.0551 0.475716 43.9929C0.343036 67.9418 19.6481 87.4569 43.5859 87.5895L44.0724 0.882774Z";
    const width1=44; const height1=88;
    const path2="M59.5084 117.483C27.3444 117.306 1.4164 91.08 1.59331 58.916C1.77021 26.752 27.9968 0.823998 60.1607 1.00091";
    const width2=60; const height2=119;
    export let style: string = "";
</script>
<div class="{style}">
    <div class="relative">
        <Svg path={path2} width={width2} height={height2} strokeWidth={2} style="text-[#1D262D]"/>
        <Svg path={path1} width={width1} height={height1} style="text-[#8BD2BD] absolute top-4 right-0"/>
    </div>
</div>