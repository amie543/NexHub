<script>
	import ExpItem from './items/ExpItem.svelte';
	import WaveSvg from './items/WaveSvg.svelte';
	import logo1 from './items/Logo1.svelte';
	import logo2 from './items/Logo2.svelte';
	import logo3 from './items/Logo3.svelte';
	const datas = [
		{
			logo: logo1,
			title: 'Experienced Engineers',
			description:
				'We teach in small groups with experienced, supportive staff who are trained to understand some of the problems our students face. '
		},
		{
			logo: logo2,
			title: 'Business Consulting',
			description:
				'Our mission is to use our knowledge, skills, and networks to equip people with multiple disadvantages with the skills to gain and sustain employment'
		},
		{
			logo: logo3,
			title: 'Graduate and  job ready',
			description:
				'We are a unique training provider willing to give you all the skills and experience you need to fulfil your future career'
		}
	];
</script>

<div class="relative overflow-hidden my-10 py-5">
	<div class="absolute top-[50px] text-[#1D262D] dark:text-[#FFE031]">
		<WaveSvg style="-ml-16 overflow-hidden" />
	</div>
	<div class="absolute bottom-0 -right-1 text-[#1D262D] dark:text-[#FFE031]">
		<WaveSvg />
	</div>
	<div class="container mx-auto mt-20">
		<div class="grid grid-cols-1  md:grid-cols-3 gap-2">
			{#each datas as data}
				<ExpItem {data} style="" />
			{/each}
		</div>
	</div>
</div>
