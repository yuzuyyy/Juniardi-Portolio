<script>
  import { arrow, shuriken } from "../assets";
  export let image = arrow;
  export let text = "text";
</script>

<div class="flex items-center gap-[8px]">
  <img
    class={image === arrow ? "size-[16px]" : "size-[24px]"}
    src={image}
    alt=""
  />
  <p class="body-1 text-white/80 capitalize">{text}</p>
</div>
