<script>
    import "../app.css";
    import { ModeWatcher } from "mode-watcher";
    import Navbar from "$lib/components/Navbar.svelte";
</script>

<Navbar />

<ModeWatcher />
<slot></slot>
