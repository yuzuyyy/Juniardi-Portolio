<script>
    import { NavItem } from ".";
    import { navItems } from "../constants";
    import MainButton from "./MainButton.svelte";
    import ToggleMenu from "./ToggleMenu.svelte";
    import { isOpen } from "../stores/isOpen";
    import { slide, fade } from 'svelte/transition';

    $: $isOpen;
</script>

<nav class="fixed   z-50 bg-primary w-full top-0 padding-x py-[10px]">
    <div class="relative section-container flex items-center justify-between">
        <div>
            <a href="/" class="font-alfa text-3xl uppercase">hw</a>
        </div>

        <!-- Desktop Nav -->
        <div class="flex items-center gap-[24px] max-md:hidden">
            {#each navItems as item}
                <NavItem {...item} />
            {/each}
        </div>

        <!-- Right buttons -->
        <div class="flex items-center gap-4">
            <MainButton
                className="rounded-full py-[5px] px-[16px] body-2 w-fit max-md:hidden"
            >
                Contact me
            </MainButton>
            <ToggleMenu />
        </div>

        <!-- Mobile Menu -->
        
            {#if $isOpen}
                <div
                    in:slide
                    out:fade
                    class="absolute rounded-3xl  bg-black text-white top-[60px] left-0 w-full z-50 flex flex-col items-center gap-6 p-6 shadow-md md:hidden"
                >
                    {#each navItems as item}
                        <NavItem {...item} />
                    {/each}
                    <MainButton className="bg-primary font-bold text-black body-1 w-full py-4">Contact me</MainButton>
                </div>
            {/if}
        


    </div>
</nav>
