<script>
    export let number = "200";
    export let simbol = "+";
    export let text = "clients";
  </script>
  
  <div class="flex flex-col  max-md:items-center w-fit">
    <p class="text-[80px] max-lg:text-[64px] max-md:text-[40px] text-textMid font-bold">
      {number}<span class="text-primary">{simbol}</span>
    </p>
    <p class="text-textMid body-1 capitalize">{text}</p>
  </div>
  