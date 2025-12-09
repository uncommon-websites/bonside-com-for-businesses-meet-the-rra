<script lang="ts">
  export let className = "";
</script>

<header class="w-full flex justify-between items-center px-6 py-4 max-w-7xl mx-auto {className}">
  <div class="flex items-center gap-12">
    <!-- Logo -->
    <a href="/" class="text-xl font-bold tracking-tight text-[#0B0F19]">BONSIDE</a>
    
    <!-- Navigation -->
    <nav class="hidden md:flex items-center gap-8">
      <a href="#" class="text-sm font-medium text-gray-700 hover:text-black">Scorecards</a>
      <a href="#" class="text-sm font-medium text-gray-700 hover:text-black">The RRA</a>
      <a href="#" class="text-sm font-medium text-gray-700 hover:text-black">Economy</a>
    </nav>
  </div>

  <!-- Actions -->
  <div class="flex items-center gap-6">
    <a href="#" class="text-sm font-medium text-gray-700 hover:text-black">Login</a>
    <a href="#" class="bg-[#0B0F19] text-white text-sm font-medium px-4 py-2 rounded-md hover:bg-gray-800 transition-colors">
      Apply
    </a>
  </div>
</header>
