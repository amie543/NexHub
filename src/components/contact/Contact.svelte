<script lang="ts">
    import ContactItem from "./items/contactItem.svelte";
    import ChatItem from "./items/chatItem.svelte";

</script>
<div class="relative my-20">
    <div class="container mx-auto">
        <div class="flex flex-row text-white bg-[#afeeee] rounded-[2px] relative">
            <ContactItem header="Contact Us" title="Improve Your Business Contact Us Now"  style="flex-1 font-poppins px-[100px] py-[60px]"/>
            <ChatItem style="flex-1  " message1="Why should I need to contact nexus hub?" message2="Because we always want our student to be updated with latest information. 😊"/>
        </div>        
    </div>
</div>