<script lang="ts">
    import SendItem from "./sendItem.svelte";
    import img from "../images/image.png" ;
    export let style: string;
    export let message1: string;
    export let message2: string;
</script>
<div class="{style} justify-evenly flex flex-col">
    <div class="bg-[#63AFB5] w-[290px] h-[340px] absolute right-[250px] bottom-0  ">
        <div class="w-[190px] h-[60px] bg-[#706982] rounded-r-[15px] rounded-bl-[15px] absolute top-10 left-10">
            <div class="text-[12px] tracking-[1%] font-[600] leading-[18px] pl-6 pr-10 pt-3 ">{message1}</div>
        </div>
        <div class="w-[240px] h-[120px] bg-[#FFFFFF] rounded-bl-[30px] rounded-t-[30px] absolute top-[120px] -right-[50px]">
            <div class="text-[13px] tracking-[1%] text-black font-[400] leading-[24px] pl-6 pr-10 pt-3">{message2}</div>
            <div class="absolute  bottom-0 -right-12">
                <div class="bg-[#2986cc] w-[40.34px] h-[40px]  rounded-full cursor-pointer select-none ">
                    <img src={img} alt=""   class="pt-1 overflow-hidden w-36 h-41 pl-1 rounded-full">
                </div>
            </div>
        </div>
         
        <div class="absolute bottom-8 left-10 ">
            <input class="w-[243x] h-[53px] placeholder:text-[#356E63]  bg-transparent  border  border-[#687687] focus:border-sky-500 outline-0 focus:ring-sky-500 focus:ring-1 sm:text-sm md:rounded-[30px] py-2 pl-8 pr-3  placeholder:tracking-[2%] placeholder:leading-[19.5px]  bottom-0 left-2  relative" placeholder="Write message" type="text" />
            <div class="absolute  bottom-[6px] right-1">
                <div class="bg-white w-[40.34px] h-[40px]  rounded-full cursor-pointer select-none ">
                    <SendItem style="text-[#367166] absolute top-1 -left-1"/>
                </div>
            </div>
        </div>
            
        </div>  
    </div>
