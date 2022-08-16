<script lang="ts">
    import Icon from 'icon/Icon.svelte';
    import { mdiCheckCircleOutline } from 'const/Icon';
    export let style: string="";
</script>
<div class="{style} flex flex-row justify-between items-center p-3 w-fit bg-white rounded-lg">
    <div class="w-[40px] h-[40px] rounded-md bg-[#3C50E0] flex flex-col justify-center items-center text-white">
        <Icon path={mdiCheckCircleOutline} size={25} />
    </div>
    <div class="flex flex-col justify-between font-inter ml-2">
        <div class="text-[#04004D] text-[14px] font-[600]">Congratulations</div>
        <div class="text-[#898E92] text-[12px]">Your admission completed</div>
    </div>
</div>