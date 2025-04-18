<script>
  import { Button, IconBox } from ".";
  import { hero } from "../assets";
  import { socmeds } from "../constants";
</script>

<section
  class="relative lg:min-h-screen bg-primary section-padding flex flex-col items-center gap-[10px]"
>
  <Button
    className="absolute max-md:hidden animate-bounce rounded-full left-[200px] top-[200px] bg-white text-black py-4 px-6 button-text"
    >Floatiing
  </Button>
  <div class="section-container w-full">
    <Button
      className="absolute max-md:hidden animate-bounce rounded-full right-[400px] bottom-[300px] bg-white text-black py-4 px-6 button-text"
      >Floatiing
    </Button>
    <div class="section-container w-full">
      <h1
        class="text-center text-[275px] max-lg:text-[140px] max-md:text-[80px] font-semibold leading-[1em]"
      >
        Hendra.work
      </h1>

      <!-- bottom start -->
      <div
        class="flex items-center justify-between w-full -mt-[50px] max-lg:-mt-[60px] max-md:-mt-[20px] max-md:flex-col max-md:items-center"
      >
        <div
          class="flex flex-col gap-[32px] self-end max-w-[240px] max-lg:w-[220px] max-lg:gap-[16px] max-md:hidden lg:pb-[24px]"
        >
          <h4 class="heading-4">
            Hello! I'm Andrea Cruz, a creative product designer based in London.
          </h4>
          <Button className="rounded-full py-[10px] px-[24px] button-text w-fit"
            >See my projects</Button
          >
        </div>

        <div class="p-[10px] bg-primary flex rounded-[48px] overflow-hidden">
          <img
            class="min-h-[440px] max-md:h-[360px] w-[400px] max-md:w-full rounded-[40px]"
            src={hero}
            alt="hero"
          />
        </div>

        <div class="flex gap-[10px] pb-[24px] self-end max-md:hidden">
          {#each socmeds as socmed (socmed)}
            <IconBox {...socmed} />
          {/each}
        </div>
      </div>
      <!-- bottom end -->

      <div class="flex flex-col items-center gap-[24px] w-full md:hidden">
        <div class="flex flex-col items-center gap-[10px] w-full">
          <h2 class="heading-4 text-center">
            Hello! I'm Andrea Cruz, a creative product designer based in London.
          </h2>
          <Button className="rounded-full py-[10px] px-[24px] button-text w-fit"
            >Contact me</Button
          >
        </div>
        <div class="flex gap-[10px]">
          {#each socmeds as socmed (socmed)}
            <IconBox {...socmed} />
          {/each}
        </div>
      </div>
      <!-- mobile content end -->
    </div>
    <!-- mobile content start-->
  </div>
</section>
