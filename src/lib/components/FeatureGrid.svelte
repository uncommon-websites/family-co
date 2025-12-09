<script>
  import Card from './Card.svelte';
</script>

<section class="py-20 px-4">
  <div class="container mx-auto max-w-6xl">
    <h2 class="text-3xl md:text-5xl font-bold text-center mb-16 tracking-tight">Explore Ethereum in a whole new way.</h2>
    
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
      
      <!-- Card 1: Send (Dark) -->
      <div class="bg-black text-white rounded-3xl p-8 flex flex-col justify-between h-full min-h-[320px] col-span-1 lg:row-span-2">
        <div class="space-y-4">
          <div class="flex items-center gap-4 bg-gray-900/50 p-3 rounded-2xl border border-gray-800">
            <div class="w-10 h-10 bg-blue-500 rounded-full flex items-center justify-center">
              <svg class="w-5 h-5 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 10l7-7m0 0l7 7m-7-7v18"></path></svg>
            </div>
            <div>
              <div class="font-bold">Send</div>
              <div class="text-xs text-gray-400">Send tokens or collectibles to any address or ENS username.</div>
            </div>
          </div>
          
          <div class="flex items-center gap-4 p-3 rounded-2xl opacity-50">
            <div class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center">
              <svg class="w-5 h-5 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7h12m0 0l-4-4m4 4l-4 4m0 6H4m0 0l4 4m-4-4l4-4"></path></svg>
            </div>
            <div>
              <div class="font-bold">Swap</div>
              <div class="text-xs text-gray-400">Swap your tokens without ever leaving your wallet.</div>
            </div>
          </div>

          <div class="flex items-center gap-4 p-3 rounded-2xl opacity-50">
             <div class="w-10 h-10 bg-gray-800 rounded-full flex items-center justify-center">
              <svg class="w-5 h-5 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path></svg>
            </div>
            <div>
              <div class="font-bold">Receive</div>
              <div class="text-xs text-gray-400">Receive Ethereum based assets through your unique address.</div>
            </div>
          </div>
        </div>
        
        <div class="mt-8">
          <h3 class="font-bold text-lg">Cozy</h3>
          <p class="text-gray-400 text-sm mt-2">Whether you're a beginner or seasoned pro, Family makes it easy.</p>
        </div>
      </div>

      <!-- Card 2: Secure -->
      <Card className="min-h-[320px]">
        <div class="flex justify-center items-center flex-grow">
          <button class="bg-green-500 text-white px-6 py-2 rounded-full font-bold shadow-lg shadow-green-200 flex items-center gap-2">
            <div class="w-2 h-2 bg-white rounded-full animate-pulse"></div>
            Backing Up
          </button>
        </div>
        <div>
          <h3 class="font-bold text-lg">Secure</h3>
          <p class="text-gray-500 text-sm mt-2">Your crypto, your control. Security at every stage.</p>
        </div>
      </Card>

      <!-- Card 3: Fast -->
      <Card className="min-h-[320px]">
        <div class="space-y-3 mb-4">
          <div class="flex items-center gap-2 text-xs text-blue-500">
            <div class="w-4 h-4 rounded-full border border-blue-500 flex items-center justify-center">✓</div>
            <span class="font-medium">Submitted</span>
            <span class="ml-auto text-gray-300">Dec 9 2023</span>
          </div>
          <div class="flex items-center gap-2 text-xs text-blue-500">
             <div class="w-4 h-4 rounded-full border border-blue-500 flex items-center justify-center">✓</div>
            <span class="font-medium">Pending</span>
          </div>
           <div class="flex items-center gap-2 text-xs text-blue-500">
             <div class="w-4 h-4 rounded-full border border-blue-500 flex items-center justify-center">✓</div>
            <span class="font-medium">Completed</span>
             <span class="ml-auto text-gray-300">Dec 9 2023</span>
          </div>
        </div>
        <div>
          <h3 class="font-bold text-lg">Fast</h3>
          <p class="text-gray-500 text-sm mt-2">Uncompromising speed. Optimal performance, all the time.</p>
        </div>
      </Card>

      <!-- Card 4: Powerful -->
      <Card className="min-h-[320px]">
        <div class="flex justify-center items-center flex-grow">
           <div class="bg-white p-4 rounded-xl shadow-sm border border-gray-100 text-center">
             <div class="text-xs text-gray-400 uppercase tracking-wide">Urgent</div>
             <div class="text-2xl font-bold text-gray-900">≈ 19 Secs</div>
             <div class="flex justify-center mt-2 gap-1">
               <div class="w-1 h-1 bg-red-400 rounded-full"></div>
                <div class="w-1 h-1 bg-orange-400 rounded-full"></div>
                 <div class="w-1 h-1 bg-green-400 rounded-full"></div>
             </div>
           </div>
        </div>
        <div>
          <h3 class="font-bold text-lg">Powerful</h3>
          <p class="text-gray-500 text-sm mt-2">Experience the full power of Ethereum with advanced features.</p>
        </div>
      </Card>

      <!-- Card 5: Fun -->
      <Card className="min-h-[320px]">
        <div class="flex justify-center items-center flex-grow -space-x-2">
           <div class="w-12 h-12 rounded-full bg-pink-400 border-2 border-white"></div>
           <div class="w-12 h-12 rounded-full bg-blue-400 border-2 border-white"></div>
           <div class="w-12 h-12 rounded-full bg-yellow-400 border-2 border-white"></div>
           <div class="w-12 h-12 rounded-full bg-purple-400 border-2 border-white"></div>
        </div>
        <div>
          <h3 class="font-bold text-lg">Fun</h3>
          <p class="text-gray-500 text-sm mt-2">Family takes fun seriously. Delightful interactions with every tap.</p>
        </div>
      </Card>

    </div>
  </div>
</section>
