<script lang="ts">
    import MapAndSocial from "./items/MapAndSocial.svelte";
    const datas=[
        {
            title: 'Pages',
            navItems: [{name: 'Home',to: '#'},{name: 'Ablut Us',to: '#'},{name: 'Courses',to: '#'},{name: 'Blog',to: '#'}]
        },
        {
            title: 'Resources',
            navItems: [{name: 'Our Location',to: '#'},{name: 'Member Stories',to: '#'}]
        },
        {
            title: 'Company',
            navItems: [{name: 'Patnerships',to: '#'},{name: 'Terms of use',to: '#'},{name: 'Privacy',to: '#'},{name: 'Sitemap',to: '#'}]
        },
    ];
</script>
<div class="mx-8 py-10 lg:mx-20 flex flex-col md:flex-row">
    {#each datas as data}
        <div class="flex-1 mt-10 md:mt-0">
            <div class="text-[20px] font[700] text-[#1C1C1D] dark:text-white">{data.title}</div>
            <div class="mt-6 leading-10 text-[16px] text-[#7A7A7E] dark:text-[#BFBFBF]">
                {#each data.navItems as item}
                    <a href={item.to} class="block cursor-pointer select-none hover:opacity-70">
                        {item.name}
                    </a>
                {/each}
            </div>
        </div>
    {/each}
    <MapAndSocial style="flex-1"/>
</div>