<script>
  import PhoneMockup from './PhoneMockup.svelte';
</script>

<section class="py-24 px-4 bg-white">
  <div class="container mx-auto max-w-6xl">
    <div class="mb-16">
      <h2 class="text-4xl md:text-5xl font-bold tracking-tight mb-4">
        Effortless onboarding.<br />
        Masterful management.
      </h2>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      
      <!-- Onboarding -->
      <div class="flex flex-col items-center">
        <PhoneMockup screenClass="bg-white flex flex-col">
          <div class="p-6 pt-12 flex-1 flex flex-col items-center justify-center text-center">
             <div class="w-16 h-16 bg-green-100 text-green-500 rounded-full flex items-center justify-center mb-6">
               <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4v16m8-8H4"></path></svg>
             </div>
             
             <h3 class="font-bold text-xl mb-2">Add an Existing Wallet</h3>
             <p class="text-gray-500 text-sm mb-6">Choose how you'd like to import an existing wallet into Family.</p>
             
             <div class="w-full bg-gray-50 p-4 rounded-xl flex items-center gap-3 text-left border border-gray-100">
               <div class="w-8 h-8 bg-green-500 rounded-full flex items-center justify-center text-white text-xs">S</div>
               <div>
                 <div class="font-bold text-sm">Secret Recovery Phrase</div>
                 <div class="text-xs text-gray-500">12, 18, or 24 words</div>
               </div>
             </div>
          </div>
        </PhoneMockup>
        <div class="mt-6 flex items-center gap-2 text-green-500 font-medium">
          <div class="w-4 h-4 rounded-full border border-green-500 flex items-center justify-center text-[10px]">✓</div>
          Onboarding
        </div>
      </div>

      <!-- Mission Control -->
      <div class="flex flex-col items-center">
        <PhoneMockup screenClass="bg-white flex flex-col">
          <div class="p-6 pt-12 flex-1">
             <div class="flex justify-between items-center mb-6">
               <div class="font-bold text-lg">Wallets</div>
               <div class="w-8 h-8 bg-gray-100 rounded-full flex items-center justify-center">+</div>
             </div>
             
             <div class="grid grid-cols-2 gap-3">
               <div class="bg-blue-500 text-white p-3 rounded-2xl aspect-square flex flex-col justify-between">
                 <div class="w-8 h-8 bg-white/20 rounded-full flex items-center justify-center">☁️</div>
                 <div>
                   <div class="font-bold text-sm">Spending</div>
                   <div class="text-xs opacity-80">$1,393.94</div>
                 </div>
               </div>
               
               <div class="bg-purple-500 text-white p-3 rounded-2xl aspect-square flex flex-col justify-between">
                 <div class="w-8 h-8 bg-white/20 rounded-full flex items-center justify-center">👾</div>
                 <div>
                   <div class="font-bold text-sm">Gaming</div>
                   <div class="text-xs opacity-80">$450.21</div>
                 </div>
               </div>

               <div class="bg-orange-500 text-white p-3 rounded-2xl aspect-square flex flex-col justify-between">
                 <div class="w-8 h-8 bg-white/20 rounded-full flex items-center justify-center">🔒</div>
                 <div>
                   <div class="font-bold text-sm">Vault</div>
                   <div class="text-xs opacity-80">$12,405</div>
                 </div>
               </div>

               <div class="bg-gray-100 text-gray-900 p-3 rounded-2xl aspect-square flex flex-col justify-between">
                 <div class="w-8 h-8 bg-white rounded-full flex items-center justify-center">👀</div>
                 <div>
                   <div class="font-bold text-sm">Watching</div>
                   <div class="text-xs text-gray-500">3 Wallets</div>
                 </div>
               </div>
             </div>
          </div>
        </PhoneMockup>
        <div class="mt-6 flex items-center gap-2 text-orange-400 font-medium">
           <div class="w-4 h-4 rounded-sm bg-orange-400 flex items-center justify-center text-white text-[10px]">::</div>
          Mission Control
        </div>
      </div>

      <!-- Drag and Drop -->
      <div class="flex flex-col items-center">
        <PhoneMockup screenClass="bg-white flex flex-col">
          <div class="p-6 pt-12 flex-1 relative">
             <div class="flex items-center gap-3 mb-6">
               <div class="w-10 h-10 bg-gray-200 rounded-full"></div>
               <div>
                 <div class="font-bold">Benji</div>
                 <div class="text-xs text-gray-500">@benjitaylor</div>
               </div>
             </div>

             <div class="space-y-3">
               <div class="flex items-center gap-3 p-3 bg-white border border-gray-100 rounded-xl shadow-sm">
                 <div class="w-8 h-8 bg-black rounded-full"></div>
                 <div class="flex-1 font-bold text-sm">Ethereum</div>
                 <div class="font-bold text-sm">$1,593.15</div>
               </div>

               <div class="flex items-center gap-3 p-3 bg-white border border-gray-100 rounded-xl shadow-sm opacity-50">
                 <div class="w-8 h-8 bg-blue-500 rounded-full"></div>
                 <div class="flex-1 font-bold text-sm">USDC</div>
                 <div class="font-bold text-sm">$2,535.04</div>
               </div>
             </div>

             <!-- Dragging Element -->
             <div class="absolute top-1/2 left-8 right-8 bg-white p-3 rounded-xl shadow-xl border-2 border-red-500 rotate-3 z-10 flex items-center gap-3">
                <div class="w-8 h-8 bg-green-500 rounded-full"></div>
                 <div class="flex-1 font-bold text-sm">Tether</div>
                 <div class="font-bold text-sm">$500.00</div>
             </div>
          </div>
        </PhoneMockup>
        <div class="mt-6 flex items-center gap-2 text-red-500 font-medium">
          <div class="w-4 h-4 border border-red-500 rounded flex items-center justify-center text-[10px]">□</div>
          Drag and Drop
        </div>
      </div>

    </div>
  </div>
</section>
