<script>
    import TextButton from "components/TextButtonComponent.svelte";
    import { dark } from "stores/store";
    let isDark = false;
    let old={};
    dark.subscribe(dark=>{
        isDark=dark;
    });
    const update = ()=> {
        dark.set(!isDark);
    }
</script>
<div class="flex flex-row justify-between h-28 w-screen px-32">
    <div class="flex flex-row flex-1 justify-start py-10">
        <img class="bg-contain aspect-[6/1]" src="/assets/logo.png" alt="nexus hub">
    </div>
    <div class="hidden md:flex flex-[2] ">
        <div class="flex flex-row flex-grow justify-center items-center space-x-10">
            <a class="text-center text-lg" href="/">Home</a>
            <a class="text-center text-lg" href="/">Services</a>
            <a class="text-center text-lg" href="/">About Us</a>
        </div>
    </div>
    <div class="hidden md:flex flex-row flex-1 justify-evenly items-center delay-1000">
        <div class="flex flex-row {isDark == true ? 'justify-end' : 'justify-start'} bg-indigo-900 h-10 w-20 rounded-full p-1.5">
            <div class="h-full aspect-square bg-yellow-300 rounded-full" on:click="{()=> update()}">
                <!-- isDark = !isDark -->
            </div>
        </div>
        <TextButton text="Contact" size="sm"/>
    </div>
</div>