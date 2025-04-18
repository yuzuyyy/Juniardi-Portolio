<script>
    export let item = "text"
    export let link = ""
    import { isOpen } from "../stores/isOpen";

    function closeMenu() {
        isOpen.set(false);
    }

    $: $isOpen;

</script>

<button on:click={closeMenu}>
    <a class="body-1 capitalize hover:text-black/50 transition-all ease-in-out duration-700" href={link}>
        {item}
    </a>
</button>
