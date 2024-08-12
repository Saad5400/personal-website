<script lang="ts">
    export let date: string;
    export let title: string;
    export let company: string;
    export let delay: number = 0;
    import {reveal} from 'svelte-reveal';
</script>

<div
	use:reveal={{
		preset: 'fly',
		y: -20,
		x: 0,
		delay: delay
	}}
	class="bg-secondary text-secondary-foreground p-8 shadow-xl flex flex-col sm:flex-row items-center gap-16">
	<div class="flex flex-col min-w-32">
		<span class="text-primary font-bold">{date}</span>
		<span class="font-bold">{title}</span>
		<span>{company}</span>
	</div>
	<div>
		<slot/>
	</div>
</div>
