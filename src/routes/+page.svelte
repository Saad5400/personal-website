<script lang="ts">
    import SocialMedia from "$lib/components/SocialMedia.svelte";
    import Button from "$lib/components/ui/button/button.svelte";
    import {reveal} from 'svelte-reveal';

</script>

<svelte:head>
	<title>
		El Cato - Web Developer
	</title>
</svelte:head>

<div class="flex justify-end pb-[35rem] lg:pb-0">
	<div
		class="bg-secondary text-secondary-foreground relative w-full lg:w-[60vw] min-h-[40vh] lg:min-h-[calc(100vh-10.5rem)] flex justify-center items-center pb-32"
	>

		<!-- Info Card -->
		<div
			class="bg-[#f4ece6] dark:bg-[#303030] shadow-[0_10px_60px_-15px_rgba(0,0,0,0.7)] w-[22rem] absolute lg:start-10 lg:-translate-x-full flex flex-col items-center justify-between pt-8 gap-2 self-bottom lg:self-start translate-y-[105%] lg:translate-y-[10%] max-w-[85vw]"
		>
			<img
				use:reveal={{
					preset: 'fade',
				}}
				src="https://elcato.sb.sa/favicon.png"
				class="rounded-full w-64 grayscale sr__hide"
				alt="الصورة الشخصية"
			/>

			<div class="flex flex-col items-center gap-8">
				<h1 use:reveal={{
					preset: 'fly',
					delay: 100
				}} class="font-bold text-4xl sr__hide">El Cato</h1>
				<hr class="w-24 border-2 border-primary"/>
				<h2 class="text-2xl">Web Developer</h2>
			</div>

			<div
				class="bg-secondary text-secondary-foreground w-full flex justify-center p-2 mt-12"
			>
				<SocialMedia/>
			</div>
		</div>
		<div class="mx-10 max-w-[30rem] flex flex-col gap-8">
			<h1 id="page-title" class="text-8xl font-extrabold">Hello</h1>
			<h4 class="text-4xl">Here's who I am & what I do</h4>
			<div class="flex gap-2">
				<Button href="/resume" class="w-32">Resume</Button>
				<Button href="/projects" variant="outline" class="w-32">Projects</Button>
			</div>
			<div class="flex flex-col gap-2">
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores
					laboriosam fugiat hic enim eveniet dolore corrupti iusto quasi quidem
					maiores nostrum beatae optio est, sequi magnam laudantium autem
					officiis. Et.
				</p>
				<p>
					Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quaerat
					recusandae, vitae, nemo enim ratione corrupti ex laboriosam mollitia,
					impedit id eaque. Amet eos illum neque eligendi quisquam, similique
					hic tenetur!
				</p>
			</div>
		</div>
	</div>
</div>
