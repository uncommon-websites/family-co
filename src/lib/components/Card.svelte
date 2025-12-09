<script>
  export let className = "";
</script>

<div class={`bg-gray-50 rounded-3xl p-8 flex flex-col justify-between h-full hover:bg-gray-100 transition-colors duration-300 ${className}`}>
  <slot />
</div>
