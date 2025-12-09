<script>
  export let screenClass = "bg-white";
</script>

<div class="relative w-[300px] h-[600px] bg-black rounded-[45px] border-[10px] border-gray-900 shadow-2xl overflow-hidden">
  <!-- Notch -->
  <div class="absolute top-0 left-1/2 -translate-x-1/2 w-32 h-7 bg-black rounded-b-2xl z-20"></div>
  
  <!-- Screen -->
  <div class={`w-full h-full overflow-hidden ${screenClass}`}>
    <slot />
  </div>
</div>
