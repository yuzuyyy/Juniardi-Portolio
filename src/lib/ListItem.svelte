<script>
  import { shuriken } from "../assets";
    export let image = shuriken
    export let text = "text"
</script>

<div class="flex items-center gap-[8px]">
    <img class="size-[24px]" src={image} alt="">
    <p class="body-1 text-white/80 capitalize">{text}</p>
</div>