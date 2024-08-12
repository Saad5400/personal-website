<script lang="ts">
    import Container from "$lib/components/Container.svelte";
    import ProjectCard from "$lib/components/ProjectCard.svelte";
    import Title from "$lib/components/Title.svelte";
</script>

<svelte:head>
	<title>
		El Cato - Projects
	</title>
</svelte:head>

<Container class="flex flex-col gap-16">
    <Title title="Projects" />
    <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Provident
        natus nemo nesciunt quaerat eos molestias eveniet ratione quas nihil
        earum ullam officiis, quod sequi asperiores minima tempore illum
        recusandae neque!
    </p>
    <ProjectCard
        title="El Cato"
        subtitle="Programming courses and quizzes"
        imageSrc={[
          "/calculator/project1.png",
          "/calculator/1.png",
          "/calculator/2.png",
        ]}
    >
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut sequi totam mollitia officiis maxime similique neque aspernatur minus perferendis a quam repellendus magni, id perspiciatis consequuntur. Libero adipisci distinctio debitis!
        </p>
    </ProjectCard>
</Container>
