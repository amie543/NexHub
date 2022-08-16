<script>
    import Svg from 'icon/Svg.svelte';
    const path1="M14.6172 18.9947V29.1761L15.3381 29.8969C15.5684 30.1271 21.104 35.5394 31.8437 35.5394C42.5834 35.5394 48.119 30.1271 48.3494 29.8968L49.0703 29.1759V18.9945L53.9922 17.0258V30.6175H58.914V15.057L63.0794 13.3909L31.8437 0.896606L0.608032 13.3909L14.6172 18.9947ZM44.1484 27.0096C42.5818 28.1795 38.516 30.6175 31.8437 30.6175C25.1715 30.6175 21.1057 28.1795 19.539 27.0096V20.9633L31.8437 25.8851L44.1484 20.9633V27.0096ZM49.8268 13.3909L31.8437 20.5841L13.8607 13.3909L31.8437 6.19779L49.8268 13.3909Z";
    const width1=64; const height1=36;
    const path2="M18.9664 21.4277L15.4862 17.9475L12.3375 21.0961C12.8835 12.0855 20.3857 4.92188 29.5311 4.92188V0C17.6521 0 7.92879 9.40029 7.40609 21.1526L4.2008 17.9475L0.720703 21.4277L9.84356 30.5506L18.9664 21.4277Z";
    const width2=30; const height2=31;
    const path3="M29.2791 9.65057L20.1562 0.52771L11.0334 9.65057L14.5136 13.1308L17.6953 9.94917V13.8517C17.6953 23.3505 9.96747 31.0783 0.46875 31.0783V36.0002C12.6814 36.0002 22.6172 26.0644 22.6172 13.8517V9.94917L25.799 13.131L29.2791 9.65057Z";
    const width3=30; const height3=36;
</script>
<div>
    <div class="flex flex-row">
        <Svg path={path2} width={width2} height={height2} style="text-[#367166] dark:text-[#7DF0DB]"/>
        <Svg path={path1} width={width1} height={height1} style="text-[#5B5B5B] dark:text-white mt-2 -ml-2"/>
    </div>
    <div class="flex flex-row">
        <Svg path={path1} width={width1} height={height1} style="text-[#5B5B5B] dark:text-white"/>
        <Svg path={path3} width={width3} height={height3} style="text-[#367166] dark:text-[#7DF0DB] mt-2 -ml-2"/>
    </div>
</div>