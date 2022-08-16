<script>
import Introduce from "./items/Introduce.svelte";
import TeacherStatis from "./items/TeacherStatis.svelte";
import Learning from "./items/Learning.svelte";
import Congratulations from "./items/Congratulations.svelte";
import squareDot from "./images/square_dot.png";
</script>
<div class="relative overflow-hidden">
	<div class="absolute -right-3 bottom-[500px] md:bottom-0">
		<img src={squareDot} alt="image">
	</div>
	<div class="container mx-auto flex flex-col-reverse md:flex-row relative">
		<div class="flex-1 relative h-[500px]">
			<Congratulations style="absolute md:top-5 md:left-20"/>
			<TeacherStatis data={[33,66]} style="absolute right-10 top-0 z-50"/>
			<Learning onPress={()=>{}} style="md:absolute ml-0 mt-20 mb-12 md:my-0 left-0 top-200 bottom-0"/>
		</div>
		<div class="flex-1 md:pl-16 pt-12 pb-12 h-[500px] flex flex-col justify-center">
			<Introduce 
				title="Get the Best Class by the Best Teachers" 
				description="Get your best class and gain the great thing from the best and well qualified experienced teachers all over the world and get shinny. We are a unique training provider willing to give you all the skills and experience you need to fulfil your future career" 
				onPress={()=>{
					console.log("read more");
				}}
			/>
		</div>
	</div>
</div>