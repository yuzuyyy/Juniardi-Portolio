<script>
  
    export let onClick = () => {};
    export let className = '';
  </script>
  
  <button
   
    class={`bg-black text-white px-6 py-2 rounded-xl hover:bg-white hover:text-black border border-black transition-all duration-300 ease-in-out ${className}`}
    on:click={onClick}
  >
    <slot />
  </button>
  