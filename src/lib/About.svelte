<script>
  import { stats } from "../constants";
import {Number} from "./";


</script>
<section class="bg-bgDark section-padding">

    <!-- container start -->
    <div class="section-container w-full">
        <div class="flex items-center justify-between  w-full">
         {#each stats as stat  }
             
         <Number {...stat}/>
         {/each}
        </div>
    </div>
    <!-- container end -->
</section>