<script lang="ts">
    import Button from "$lib/components/ui/button/button.svelte";
</script>

<div class="max-w-screen-sm px-4 mx-auto pt-16">
    <h1 class="mx-auto w-fit text-4xl font-bold flex items-center">
        <div class="bg-primary w-5 h-5 me-4" />
        <span>Resume</span>
    </h1>
    <div class="pt-16 flex flex-col gap-8">
        <div class="flex justify-between items-center">
            <span class="text-2xl font-bold">Education</span>
            <Button>Download CV</Button>
        </div>
        <div class="bg-secondary p-8 shadow-xl flex items-center gap-16">
            <div class="flex flex-col min-w-32">
                <span class="text-primary font-bold">
                    2023 - present
                </span>
                <span class="font-bold">
                    Computer Science Bachelor
                </span>
                <span>
                    Umm Al-Qura University
                </span>
            </div>
            <div>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Eum
                    ipsa hic fugiat quos voluptas voluptatibus ut porro qui
                    iusto a esse corrupti, accusantium iure impedit ratione
                    maxime deserunt itaque sit?
                </p>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Adipisci vitae eveniet eaque libero animi veritatis
                    perspiciatis aspernatur corporis a veniam mollitia sint, non
                    cum nesciunt quas quam ullam! Impedit, accusamus?
                </p>
            </div>
        </div>
    </div>
</div>
