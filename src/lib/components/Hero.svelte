<script lang="ts">
  import Header from "./Header.svelte";
</script>

<section class="relative w-full bg-gradient-to-b from-[#C4D0FF] via-[#EBEFFF] to-white pb-20 overflow-hidden">
  <Header />
  
  <div class="max-w-7xl mx-auto px-6 pt-12 md:pt-20 flex flex-col items-center text-center">
    <!-- Icon -->
    <div class="mb-8">
      <svg width="40" height="24" viewBox="0 0 40 24" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M0 0H12V4H0V0Z" fill="#0B0F19"/>
        <path d="M0 10H12V14H0V10Z" fill="#0B0F19"/>
        <path d="M0 20H12V24H0V20Z" fill="#0B0F19"/>
        <path d="M14 0H26V4H14V0Z" fill="#0B0F19"/>
        <path d="M14 10H26V14H14V10Z" fill="#0B0F19"/>
        <path d="M14 20H26V24H14V20Z" fill="#0B0F19"/>
        <path d="M28 0H40V4H28V0Z" fill="#0B0F19"/>
        <path d="M28 20H40V24H28V20Z" fill="#0B0F19"/>
        <!-- Custom stylized B logo approximation -->
        <rect x="15" y="6" width="10" height="2" fill="#0B0F19"/>
        <rect x="15" y="16" width="10" height="2" fill="#0B0F19"/>
      </svg>
    </div>

    <!-- Headline -->
    <h1 class="text-4xl md:text-6xl font-semibold tracking-tight text-[#0B0F19] mb-6 max-w-3xl leading-[1.1]">
      Open your next location<br>with a Bonside RRA.
    </h1>

    <!-- Subheadline -->
    <p class="text-lg text-gray-600 mb-8 max-w-xl leading-relaxed">
      The <span class="font-semibold text-gray-900">Repeatable Revenue Agreement</span> is financing<br>tailor-made for service-based businesses.
    </p>

    <!-- CTA -->
    <a href="#" class="bg-[#0B0F19] text-white text-sm font-medium px-6 py-3 rounded-md hover:bg-gray-800 transition-colors flex items-center gap-2 mb-16">
      Apply for funding
      <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M6 12L10 8L6 4" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
    </a>

    <!-- Dashboard Card Visual -->
    <div class="w-full max-w-4xl bg-white rounded-2xl shadow-xl overflow-hidden flex flex-col md:flex-row relative z-10">
      <!-- Left Content -->
      <div class="p-8 md:w-1/2 flex flex-col justify-between">
        <div>
          <div class="flex justify-between items-start mb-1">
            <h3 class="text-xl font-semibold text-[#0B0F19]">My Bonside RRA – No. 3</h3>
            <span class="text-xs text-gray-500">Month 36</span>
          </div>
          <p class="text-gray-500 text-sm mb-6">November 2024</p>
          
          <div class="flex items-center gap-2 mb-8">
            <div class="w-2 h-2 rounded-full bg-green-500"></div>
            <span class="text-sm font-medium text-green-700">On track</span>
            <span class="text-sm text-gray-400">with estimated payouts.</span>
          </div>
        </div>

        <!-- Progress Graphic -->
        <div class="mb-8 relative">
           <!-- Custom progress bar visualization -->
           <div class="h-16 w-full flex items-end gap-1">
              <!-- This is a simplified representation of the bar chart in the screenshot -->
              <div class="w-full bg-[#0B0F19] h-8 relative rounded-sm overflow-hidden">
                <div class="absolute top-0 left-0 h-full w-[75%] bg-[#0B0F19]"></div>
                <div class="absolute top-0 right-0 h-full w-[25%] bg-[#E5E7EB]"></div>
                <!-- The teal marker -->
                <div class="absolute top-[-10px] left-[74%] w-1 h-12 bg-[#2DD4BF] z-10"></div>
              </div>
           </div>
        </div>

        <div class="flex justify-between items-end">
          <div>
            <h4 class="text-2xl font-bold text-[#0B0F19]">$752,084</h4>
            <div class="flex items-center gap-2 mt-1">
              <div class="w-2 h-2 rounded-full bg-[#0B0F19]"></div>
              <span class="text-xs text-gray-500">Paid back</span>
            </div>
          </div>
          <div class="text-right">
            <h4 class="text-2xl font-bold text-[#0B0F19] opacity-40">$1,000,000</h4>
            <div class="flex items-center gap-2 mt-1 justify-end">
              <div class="w-2 h-2 rounded-full bg-gray-300"></div>
              <span class="text-xs text-gray-400">Total financed</span>
            </div>
          </div>
        </div>
      </div>

      <!-- Right Image -->
      <div class="md:w-1/2 relative h-64 md:h-auto bg-gray-100">
        <img 
          src="https://images.unsplash.com/photo-1600607686527-6fb886090705?q=80&w=2700&auto=format&fit=crop" 
          alt="Interior" 
          class="absolute inset-0 w-full h-full object-cover"
        />
        <!-- Overlay Tags -->
        <div class="absolute top-4 left-4 flex gap-2">
          <div class="bg-white/90 backdrop-blur-sm px-2 py-1 rounded text-[10px] font-medium text-gray-800">
            Location 5
          </div>
          <div class="bg-black/60 backdrop-blur-sm px-2 py-1 rounded text-[10px] font-medium text-white">
            Opened 15 months ago
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
