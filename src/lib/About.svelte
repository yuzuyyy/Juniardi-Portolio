<script>
  import { services, stats, tools } from "../constants";
import {ListItem, Number} from "./";


</script>
<section class="bg-bgDark section-padding">

    <!-- container start -->
    <div class="section-container flex flex-col gap-[80px] w-full">
        <div class="flex items-center justify-between  w-full">
         {#each stats as stat  }
         <Number {...stat}/>
         {/each}
        </div>

        <!-- about me start -->
        <div class="grid grid-cols-2 max-lg:grid-cols-1 gap-[24px]">
            <div class="flex flex-col  lg:min-h-[280px] h-fit pt-[16px] gap-[10px]">
                <p class="body-1 text-white/80 md:max-lg:max-w-[480px]">Design, for me, goes beyond solving problems. It's about improving user experiences, striking the perfect balance between aesthetics and functionality, and even creating products that form emotional connections with users.</p>

                <p class="heading-5 text-white">Signature</p>
            </div>

            <div class="flex flex-col lg:items-end pl-[80px] max-lg:p-0 gap-[24px] lg:text-end">
                <h2 class="heading-3 text-white capitalize">My <span class="text-primary">services</span></h2>
                {#each services as service } 
                <ListItem text={service}/>
                {/each}
            </div>

            <div class="flex flex-col items-start max-lg:p-0 gap-[24px]">
                <h2 class="heading-3 text-white capitalize">Tools and <span class="text-primary">expertise</span></h2>
                {#each tools as tool } 
                <ListItem {...tool}/>
                {/each}
            </div>
        </div>
        <!-- about me end -->
    </div>
    <!-- container end -->
</section>