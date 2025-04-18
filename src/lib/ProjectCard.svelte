<script>
  import { project1 } from "../assets";
  export let image = project1
  export let title = "Title"
  export let description = "description"
</script>

<a href="">
  <div
    class="relative p-[24px] min-h-[340px] min-w-[280px] max-lg:w-full rounded-[40px] overflow-hidden group flex flex-col justify-between"
  >
    <img
      class="absolute inset-0 w-full h-full bg-cover group-hover:scale-125 transition-all ease-in-out duration-700"
      src={image}
      alt=""
    />

    <div></div>
    <div
      class="z-10 bg-white w-full rounded-full flex flex-col gap-2 py-[8px] px-[24px] group-hover:bg-primary transition-all ease-in-out duration-700"
    >
      <h6 class="heading-6">{title}</h6>
      <p class="body-1 text-black/50">{description}</p>
    </div>
  </div>
</a>
