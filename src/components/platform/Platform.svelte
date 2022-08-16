<script>
    import PlatformItem from "./items/platformItem.svelte";
    import PhotoItem from "./items/photoItem.svelte";
    import YellowRing from "./items/yellowRing.svelte";
    import ManyRings from "./items/manyRings.svelte";

</script>
<div class="my-20 relative ">
    <div class="container mx-auto">
        <div class="absolute left-[900px] bottom-0 ">
            <ManyRings style="text-blue"/>
        </div>
        <div class="absolute left-[680px] -top-[70px] ">
            <YellowRing style="text-[#FFC200]"/>
        </div>
        <div class="flex flex-col md:flex-row ">
            <div class="flex-1">
                 <PlatformItem header="SIMPLE LEAENING PLATFORM" title="A quality focus Software House for Business" description="A best and cheapest way of getting know learning to make a better tomorrow "/>
            </div>
           
            <div class="flex-1 z-[500]">
                <PhotoItem style="w-[526px] h-[656px]"/>
            </div>
        </div>
    </div>
</div>
