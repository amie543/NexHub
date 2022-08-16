<script lang="ts">
    import { onMount } from 'svelte';
    import 'const/chart/index.js';
    export let data :Array<Number>;
    export let style : string = "";
    const dataDoughnut = {
    //   labels: ["Other Sector", "IT Sector"],
      datasets: [
        {
          label: "My First Dataset",
          data,
          backgroundColor: [
            "#FAB408",
            "#19BF6F",
          ],
          hoverOffset: 4,
        },
      ],
    };
  
    const configDoughnut = {
      type: "doughnut",
      data: dataDoughnut,
      options: {},
    };
    onMount(async () => {
        var chartBar = new Chart(
            document.getElementById("chartDoughnut"),
            configDoughnut
        );
	});

</script>
<div class="w-[280px] h-[340px] p-[35px] rounded-xl bg-white font-inter flex flex-col items-center justify-between {style}">
    <div class="text-[#04004D] text-[14px] font-[600]">Teachers Statistics</div>
    <canvas class="p-6" id="chartDoughnut"></canvas>
    <div class="flex flex-row w-full">
        <div class="flex-1 flex flex-col justify-center pl-4 py-2 bg-amber-200 rounded-lg mr-1">
            <div class="text-amber-600 text-[20px]">{data[0]}%</div>
            <div class="text-amber-600 text-[8px]">Other Sector</div>
        </div>
        <div class="flex-1 flex flex-col justify-center pl-4 py-2 bg-green-200 rounded-lg ml-1">
            <div class="text-green-600 text-[20px]">{data[1]}%</div>
            <div class="text-green-600 text-[8px]">It Sector</div>
        </div>
    </div>
</div>