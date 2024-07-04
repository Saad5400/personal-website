<script lang="ts">
    import { cn } from "$lib/utils";

    export let title: string;
    let className: string = "";

    export { className as class };
</script>

<h1 class={cn("mx-auto w-fit text-4xl font-bold flex items-center", className)}>
    <div class="bg-primary w-5 h-5 me-4" />
    <span>{title}</span>
</h1>
