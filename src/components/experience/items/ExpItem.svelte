<script lang="ts">
    export let style :string = "";
    interface dataProps {
        logo : any;
        title : string;
        description : string;        
    }
    export let data : dataProps;   
</script>
<div class="{style} flex flex-col p-4  items-center text-center">
    <div>
        <svelte:component this={data.logo} />
    </div>
    <div class="font-poppins text-[24px] leading-[24px] font-[500] text-[#1E1E1E] dark:text-white mt-12">{data.title} </div>
    <div class="mt-4">{data.description}</div>

</div>