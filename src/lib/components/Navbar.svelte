<script>
    import Button from "./ui/button/button.svelte";
    import { page } from "$app/stores";
</script>

<div class="w-[100dvw] bg-secondary text-secondary-foreground py-8 px-6">
    <nav class="max-w-screen-2xl flex justify-between items-baseline mx-auto">
        <div class="flex items-center gap-2">
            <div class="bg-primary w-5 h-5 me-4" />
            <div class="flex items-end gap-1">
                <span class="font-bold text-3xl"> El Cato </span>
                <span class="text-xl uppercase"> / Web Developer </span>
            </div>
        </div>

        <div class="uppercase">
            <Button
                class=" {$page.url.pathname == '/' && 'text-primary'}"
                href="/"
                variant="link">About me</Button
            >
            <Button
                class=" {$page.url.pathname == '/resume' && 'text-primary'}"
                href="/resume"
                variant="link">Resume</Button
            >
            <Button
                class=" {$page.url.pathname == '/projects' && 'text-primary'}"
                href="/projects"
                variant="link">Projects</Button
            >
            <Button
                class=" {$page.url.pathname == '/contact' && 'text-primary'}"
                href="/contact"
                variant="link">Contact</Button
            >
        </div>
    </nav>
</div>
