<script>
    import SocialMedia from "./SocialMedia.svelte";
</script>

<footer class="bg-secondary text-secondary-foreground py-2 px-6">
    <div
        class="max-w-screen-2xl flex flex-row-reverse md:flex-row justify-between items-center mx-auto"
    >
        <span class="self-end md:self-center">
            © {new Date().getFullYear()}
        </span>
        <div class="flex flex-col md:flex-row gap-4 md:gap-16">
            <span class="flex gap-4 md:gap-0 md:flex-col items-center">
                <span class="font-bold">Call</span>
                <a href="tel:0501321169">0501321169</a>
            </span>
            <span class="flex gap-4 md:gap-0 md:flex-col items-center">
                <span class="font-bold">Email</span>
                <a href="mailto:elcato5400@gmail.com">elcato5400@gmail.com</a>
            </span>
            <span class="flex items-center">
                <SocialMedia />
            </span>
        </div>
    </div>
</footer>
