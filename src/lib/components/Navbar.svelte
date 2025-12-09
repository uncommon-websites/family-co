<script>
  import NavLink from './NavLink.svelte';
</script>

<nav class="fixed top-0 left-0 right-0 z-50 flex items-center justify-between px-6 py-4 bg-white/80 backdrop-blur-md border-b border-transparent transition-all duration-200">
  <div class="flex items-center gap-8">
    <a href="/" class="text-xl font-bold tracking-tight">Family</a>
    
    <div class="hidden md:flex items-center gap-6">
      <NavLink>Developers</NavLink>
      <NavLink>Resources</NavLink>
      <NavLink>X (Twitter)</NavLink>
    </div>
  </div>

  <div class="flex items-center gap-4">
    <a href="#" class="text-sm font-medium text-gray-600 hover:text-black transition-colors px-3 py-2">Login</a>
    <a href="#" class="text-sm font-medium text-white bg-black hover:bg-gray-800 transition-colors px-5 py-2.5 rounded-full">Get Started</a>
  </div>
</nav>
