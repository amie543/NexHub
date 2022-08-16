<script>
	import '../app.css';
    import NavigationBar from '../components/NavigationBar.svelte';
    import { dark } from '../stores/store';
    let isDark=false;
    dark.subscribe(dark=>{
        isDark=dark;
    });
</script>

<div class="bg-cover bg-[url('/assets/rectangle.png')] {isDark? 'dark':''}">
    <div class="dark:bg-[#0B315E] bg-white dark:text-white">
        <NavigationBar/>
        <slot />
    </div>
</div>
