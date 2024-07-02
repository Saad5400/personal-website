<script>
    import Button from "./ui/button/button.svelte";
</script>

<nav
    class="flex justify-between w-[100dvw] bg-secondary text-secondary-foreground py-8 px-4"
>
    <div class="flex items-center gap-2 text-3xl">
        <div class="bg-primary w-5 h-5 me-4" />
        <span class="font-bold"> El Cato </span>
        <span class="text-2xl"> / Web Developer </span>
    </div>

    <div>
        <Button href="/" variant="link">About me</Button>
        <Button href="/resume" variant="link">Resume</Button>
        <Button href="/projects" variant="link">Projects</Button>
        <Button href="/contact" variant="link">Contact</Button>
    </div>
</nav>
