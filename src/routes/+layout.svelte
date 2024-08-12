<script>
    import "../app.css";
    import "svelte-reveal/styles.css";
    import { ModeWatcher } from "mode-watcher";
    import Navbar from "$lib/components/Navbar.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import { onNavigate } from '$app/navigation';

    onNavigate((navigation) => {
        // @ts-ignore
        if (!document.startViewTransition) return;

        return new Promise((resolve) => {
            // @ts-ignore
            document.startViewTransition(async () => {
                resolve();
                await navigation.complete;
            });
        });
    });
</script>

<Navbar />

<ModeWatcher />

<main class="min-h-[calc(100vh-10.5rem)]">
    <slot />
</main>

<Footer />
