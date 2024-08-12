<script lang="ts">
    import * as Carousel from "$lib/components/ui/carousel/index.js";
    import Autoplay from "embla-carousel-autoplay";

    export let title: string;
    export let subtitle: string;
    export let imageSrc: string[];
</script>

<div class="bg-secondary text-secondary-foreground shadow-xl flex flex-col gap-4 justify-between">
	<div class="flex flex-col gap-16 pt-8">
		<div class="flex flex-col min-w-32 border-s-8 border-primary ps-8">
			<span class="font-bold text-primary text-xl">{title}</span>
			<span>{subtitle}</span>
		</div>
		<div class="px-8 pb-4">
			<slot/>
		</div>
	</div>
	<Carousel.Root
		opts={{
			loop: true
		}}
		plugins={[
			Autoplay({
				delay: 2000,
			}),
		]}
	>
		<Carousel.Content>
			{#each imageSrc as src}
				<Carousel.Item class="flex justify-center items-center">
					<img src={src} alt="صورة المشروع" class="w-auto object-cover"/>
				</Carousel.Item>
			{/each}
		</Carousel.Content>
	</Carousel.Root>
</div>
