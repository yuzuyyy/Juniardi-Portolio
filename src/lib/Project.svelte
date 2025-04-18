<script>
  import { ProjectCard } from ".";


</script>

<section class="bg-white/80 w-full section-padding ">

    <div class="w-full flex flex-col gap-[40px] max-md:gap-[24  section-container">
        <div>
            <h1 class="heading-1 text-black">My projects</h1>
        </div>

        <div class=" grid grid-cols-1 md-grid-cols-2 lg:grid-cols-3 gap-[24px]">
            <ProjectCard />
            <ProjectCard />
            <ProjectCard />
        </div>
    </div>
   
</section>