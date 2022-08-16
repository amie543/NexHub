<script lang="ts">
    import PackageCard from "./items/PackageCard.svelte";
    import image1 from "./images/image1.png";
    import image2 from "./images/image2.png";
    import image3 from "./images/image3.png";
    const datas = [
        {
            image: image1,
            title: "A Complete Web development",
            subTitle: "Technology > Web development",
            dashboard: {
                price: 450,
                hour: 23.5,
                article: 52
            }
        },
        {
            image: image2,
            title: "Music Production Courses",
            subTitle: "Music & Sounding",
            dashboard: {
                price: 320,
                hour: 18.5,
                article: 27
            }
        },
        {
            image: image1,
            title: "Personality development course",
            subTitle: "Personal development",
            dashboard: {
                price: 620,
                hour: 32.3,
                article: 37
        }
    }
    ];
</script>
<div class="py-20">
    <div class="container mx-auto">
        <div class="text-[35px]">Featured Packages</div>
        <div class="text-[#BDBDBD] text-[16px] my-2">Everything you need is to choose a package.</div>
        <div class="mt-10 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 md:gap-8 lg:gap-12">
            {#each datas as data}
                <PackageCard {data}/>
            {/each}
        </div>
    </div>
</div>