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
    <div class="flex flex-row justify-evenly mt-4 text-gray-800 my-5">
        <div>${data.dashboard.price}</div>
        <div class="">
            <Icon path={mdiMonitor} size={20}/>
            {data.dashboard.hour} hours
        </div>
        <div>
            <Icon path={mdiFileOutline} size={20}/>
            {data.dashboard.article}
            Articles
        </div>
    </div>
</div>