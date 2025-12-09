<script lang="ts">
  const portfolioItems = [
    {
      name: "Y7 Studio",
      locations: "9 locations",
      cities: "3 cities",
      image: "https://images.unsplash.com/photo-1599447421405-0c323d216d1b?q=80&w=600&auto=format&fit=crop",
      logo: true
    },
    {
      name: "Nimbus Kitchen",
      locations: "5 locations",
      cities: "2 cities",
      image: "https://images.unsplash.com/photo-1556910103-1c02745a30bf?q=80&w=600&auto=format&fit=crop",
      logo: false
    },
    {
      name: "Matchaful",
      locations: "8 locations",
      cities: "New York City",
      image: "https://images.unsplash.com/photo-1554118811-1e0d58224f24?q=80&w=600&auto=format&fit=crop",
      logo: false
    },
    {
      name: "Broad Street Oyster Co.",
      locations: "7 locations",
      cities: "California",
      image: "https://images.unsplash.com/photo-1559339352-11d035aa65de?q=80&w=600&auto=format&fit=crop",
      logo: false
    },
    {
      name: "José Andrés Group",
      locations: "8 cities",
      cities: "16 locations",
      image: "https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?q=80&w=600&auto=format&fit=crop",
      logo: false
    }
  ];

  const categories = [
    { name: "Hospitality", icon: "cup" },
    { name: "Wellness", icon: "heart" },
    { name: "Services", icon: "wrench" },
    { name: "Fitness", icon: "dumbbell" },
    { name: "Entertainment", icon: "ticket" },
    { name: "Petcare", icon: "home" }
  ];
</script>

<section class="py-24 bg-white overflow-hidden">
  
  <!-- Carousel -->
  <div class="flex gap-4 overflow-x-auto pb-12 px-6 md:px-[calc((100vw-1280px)/2+1.5rem)] no-scrollbar">
    {#each portfolioItems as item}
      <div class="flex-none w-[280px] h-[280px] relative rounded-lg overflow-hidden group cursor-pointer">
        <img src={item.image} alt={item.name} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
        <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent to-transparent"></div>
        
        {#if item.logo}
          <div class="absolute inset-0 flex items-center justify-center">
             <h3 class="text-white text-3xl font-bold italic opacity-80">{item.name}</h3>
          </div>
        {/if}

        <div class="absolute bottom-4 left-4 text-white">
          <h4 class="font-bold text-sm mb-0.5">{item.name}</h4>
          <p class="text-[10px] opacity-80">{item.locations}</p>
          <p class="text-[10px] opacity-80">{item.cities}</p>
        </div>
      </div>
    {/each}
    <!-- Peek of next card -->
     <div class="flex-none w-[100px] h-[280px] relative rounded-lg overflow-hidden">
        <img src="https://images.unsplash.com/photo-1509042239860-f550ce710b93?q=80&w=600&auto=format&fit=crop" alt="More" class="w-full h-full object-cover opacity-50" />
     </div>
  </div>

  <div class="max-w-7xl mx-auto px-6 text-center">
    <h2 class="text-3xl md:text-4xl font-semibold text-[#0B0F19] mb-8">
      Backing best-in-class businesses.
    </h2>

    <div class="flex flex-wrap justify-center gap-x-8 gap-y-4 mb-12">
      {#each categories as cat}
        <div class="flex items-center gap-2 text-sm font-medium text-[#0B0F19]">
          <!-- Simple Icon Placeholder -->
          <span class="w-4 h-4 bg-[#0B0F19] rounded-full flex items-center justify-center text-[8px] text-white">
             {#if cat.icon === 'cup'}H
             {:else if cat.icon === 'heart'}W
             {:else if cat.icon === 'wrench'}S
             {:else if cat.icon === 'dumbbell'}F
             {:else if cat.icon === 'ticket'}E
             {:else if cat.icon === 'home'}P
             {/if}
          </span>
          {cat.name}
        </div>
      {/each}
    </div>

    <a href="#" class="inline-flex items-center gap-2 bg-[#0B0F19] text-white text-sm font-medium px-6 py-3 rounded-md hover:bg-gray-800 transition-colors">
      See the portfolio
      <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M6 12L10 8L6 4" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
    </a>
  </div>
</section>

<style>
  .no-scrollbar::-webkit-scrollbar {
    display: none;
  }
  .no-scrollbar {
    -ms-overflow-style: none;
    scrollbar-width: none;
  }
</style>
