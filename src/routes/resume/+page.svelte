<script lang="ts">
	import Button from "$lib/components/ui/button/button.svelte";
	import ResumeCard from "$lib/components/ResumeCard.svelte";
	import Title from "$lib/components/Title.svelte";
	import Container from "$lib/components/Container.svelte";
  import {reveal} from 'svelte-reveal';
</script>

<svelte:head>
	<title>
		El Cato - Resume
	</title>
</svelte:head>


<Container>
	<Title title="Resume" />
	<div class="pt-16 flex flex-col gap-8">
		<div class="flex justify-between items-center">
			<span class="text-2xl font-bold">Education</span>
			<Button>Download CV</Button>
		</div>
		<ResumeCard
			date="2023 - present"
			title="Computer Science Bachelor"
			company="Umm Al-Qura University"
		>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum
				ipsa hic fugiat quos voluptas voluptatibus ut porro qui iusto a
				esse corrupti, accusantium iure impedit ratione maxime deserunt
				itaque sit?
			</p>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit.
				Adipisci vitae eveniet eaque libero animi veritatis perspiciatis
				aspernatur corporis a veniam mollitia sint, non cum nesciunt
				quas quam ullam! Impedit, accusamus?
			</p>
		</ResumeCard>
		<ResumeCard
			date="2023 - present"
			title="Computer Science Bachelor"
			company="Umm Al-Qura University"
		>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum
				ipsa hic fugiat quos voluptas voluptatibus ut porro qui iusto a
				esse corrupti, accusantium iure impedit ratione maxime deserunt
				itaque sit?
			</p>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit.
				Adipisci vitae eveniet eaque libero animi veritatis perspiciatis
				aspernatur corporis a veniam mollitia sint, non cum nesciunt
				quas quam ullam! Impedit, accusamus?
			</p>
		</ResumeCard>
		<ResumeCard
			date="2023 - present"
			title="Computer Science Bachelor"
			company="Umm Al-Qura University"
		>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum
				ipsa hic fugiat quos voluptas voluptatibus ut porro qui iusto a
				esse corrupti, accusantium iure impedit ratione maxime deserunt
				itaque sit?
			</p>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit.
				Adipisci vitae eveniet eaque libero animi veritatis perspiciatis
				aspernatur corporis a veniam mollitia sint, non cum nesciunt
				quas quam ullam! Impedit, accusamus?
			</p>
		</ResumeCard>
		<ResumeCard
			date="2023 - present"
			title="Computer Science Bachelor"
			company="Umm Al-Qura University"
		>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum
				ipsa hic fugiat quos voluptas voluptatibus ut porro qui iusto a
				esse corrupti, accusantium iure impedit ratione maxime deserunt
				itaque sit?
			</p>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit.
				Adipisci vitae eveniet eaque libero animi veritatis perspiciatis
				aspernatur corporis a veniam mollitia sint, non cum nesciunt
				quas quam ullam! Impedit, accusamus?
			</p>
		</ResumeCard>
		<ResumeCard
			date="2023 - present"
			title="Computer Science Bachelor"
			company="Umm Al-Qura University"
			delay={250}
		>
			<p>Hello World</p>
		</ResumeCard>
	</div>
</Container>
