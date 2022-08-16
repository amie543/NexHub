<script lang="ts">
    import Icon from 'const/Icon/Icon.svelte';
    import { mdiMonitor, mdiFileOutline } from 'const/Icon/index'
    interface DashProps {
        price: number;
        hour: number;
        article: number;
    }
    interface DataProps {
        image: string;
        title: string;
        subTitle: string;
        dashboard: DashProps;
    }
    export let data: DataProps;
    export let style: string = "";
</script>
<div class="rounded-xl bg-white">
    <div class="{style} flex flex-row">
        <img src={data.image} alt="" class="w-full">
    </div>
    <div class="mx-2 text-[17px] text-black my-2">{data.title}</div>
    <div class="mx-2 text-[14px] text-[#878787]">{data.subTitle}</div>
    <div class="mx-3 flex flex-row justify-between mt-4 text-black my-5">
        <div>
            $ <span class="text-[#4D4D52]">{data.dashboard.price}</span>
        </div>
        <div class="flex flex-row items-center">
            <Icon path={mdiMonitor} size={25} style="mr-0.5"/>
            <span class="text-[#4D4D52]">
                {data.dashboard.hour} hours
            </span>
        </div>
        <div class="flex flex-row items-center">
            <Icon path={mdiFileOutline} size={25} style="mr-1"/>
            <span class="text-[#4D4D52]">
                {data.dashboard.article}
                Articles
            </span>
        </div>
    </div>
</div>