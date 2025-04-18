<script>
    export let text = "Link";
    export let link = "#";
    import { isOpen } from "../stores/isOpen";

    function closeMenu() {
        isOpen.set(false);
    }
</script>

<a
    href={link}
    on:click={closeMenu}
    class="body-1 capitalize hover:text-white/50 transition-all duration-300"
>
    {text}
</a>
