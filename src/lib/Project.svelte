<script>
  import { MainButton, ProjectCard } from ".";
    import { projects } from "../constants";
</script>

<section class="bg-white/80 w-full section-padding">
  <div class="w-full flex flex-col gap-[40px] max-md:gap-[24px] section-container">
    <div>
      <MainButton className="w-fit button-text ">Become a client</MainButton>
    </div>

    <div class=" grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-[24px] w-full">
      {#each projects as project  }
        <ProjectCard {...project} />
      {/each}
    </div>

   
  </div>
</section>
