<script lang="ts">
    export let header:string;
    export let title:string;
    export let description:string;
    
</script>
<div class="flex flex-col font-poppins w-[500px] ">
    <div class="text-[16px] dark:text-[#BFBFBF] text-[#2F2B71] tracking-[3%]">{header}</div>
    <div class=" my-5  font-[700] text-[58px] dark:text-white leading-[72px] text-[#101130]" >{title}</div>
    <div class=" w-[350px] text-[18px] dark:text-[#BFBFBF] leading-[32px] text-[#67687B]">{description}</div>    
</div>