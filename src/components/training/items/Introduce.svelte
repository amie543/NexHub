<script lang="ts">
    import Icon from "icon/Icon.svelte"; 
    import { mdiArrowRight } from "icon/index";
    export let title:string;
    export let description:string;
    export let onPress: VoidFunction;
</script>
<div class="flex flex-col font-inter justify-between h-full mx-4 md:mx-0">
    <div class="text-[#04004D] dark:text-white text-[50px] leading-[62px] font-[700] text-center md:text-left">{title}</div>
    <div class="text-[#336C61] dark:text-gray-300 text-[16px] leading-[26px] font-[400] mt-8 text-center md:text-left">{description}</div>
    <div on:click={onPress} class="flex flex-row font-inter justify-center md:justify-start items-center mt-6 cursor-pointer select-none hover:opacity-70 text-[#336C61] dark:text-gray-300">
        <div class="text-[16px] leading-[26px] font-[400] mr-2">Read more</div>
        <Icon path={mdiArrowRight} size={30} style=""/>
    </div>
</div>