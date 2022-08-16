<script lang="ts">
    export let header:string;
    export let title:string;
    export let description:string;
    export let onPress: VoidFunction = ()=>{console.log('you click start')};
</script>
<div class="flex flex-col items-center md:items-start font-poppins md:pr-20 justify-evenly py-20">
    <div class="text-[16px] dark:text-[#BFBFBF] text-[#2F2B71] tracking-[3%]">{header}</div>
    <div class=" my-5 font-[700] text-[35px] md:text-[58px] dark:text-white md:leading-[72px] text-[#101130]" >{title}</div>
    <div class="text-[18px] dark:text-[#BFBFBF] leading-[32px] text-[#67687B]">{description}</div>
    <div on:click={onPress} class="w-[180px] h-[55px] flex flex-row justify-center items-center text-[18px] text-white rounded-sm select-none cursor-pointer dark:text-[#0B315E] bg-[#0B315E] dark:bg-[#FFE031] mt-6">
        Start Free Trial
    </div>
</div>