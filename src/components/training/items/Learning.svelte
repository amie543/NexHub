<script lang="ts">
    import image from "../images/learning.png";
    export let style: string = "";
    export let onPress: VoidFunction;
</script>
<div class="{style} w-[340px] h-[395px] p-[30px] rounded-xl bg-white font-inter flex flex-col justify-between">
    <img src={image} alt="image">
    <div class="text-[#FF733B] text-[15px]">Music Mastery</div>
    <div class="text-[#04004D] text-[24px]">Basic to higher level</div>
    <div class="text-[#898E92] text-[18px]">Class 01</div>
    <div on:click={onPress} class="flex flex-row justify-between items-center">
        <div class="text-[#898E92] text-[14px]">Today · 07.PM - 09.PM</div>
        <div class="text-white text-[12px] bg-[#367166] px-2 py-1 rounded-md cursor-pointer select-none hover:opacity-75">JOIN NOW</div>
    </div>
</div>