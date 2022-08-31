<script lang="ts">
    import LeftArrow from "./leftArrow.svelte";
    export let header :string;
    export let title :string;
    export let style: string;
</script>
<div class="{style} flex flex-col justify-evenly  " >    
    <div class="font-[500] text-[#8785AA] ledding-[22px] text-[18px] tracking-[6px] uppercase">{header}</div>
    <div class="font-[600] text-[#1B1B1B] ledding-[52px] text-[40px] pr-15 mb-10">{title}</div>
    <div class="relative ">
        <input class="w-[330px] h-[70px] placeholder:text-[#8D8A7A] bg-white border border-slate-300 rounded-sm py-2 pl-9 pr-3 shadow-sm outline-0 focus:border-sky-500 placeholder:tracking-[0.2px] placeholder:leading-[22px] placeholder:font-[500] focus:ring-sky-500 focus:ring-1 sm:text-sm" placeholder="enter your mail..." type="text" />
        <div class="absolute text-black top-3 left-[270px]">
            <div class="bg-[#12294B] w-[50px] h-[50px] cursor-pointer select-none">
                <LeftArrow style="text-white"/>
            </div>
        </div>
    </div>
</div>
