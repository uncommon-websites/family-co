<script>
  // Send, Receive, Swap section
</script>

<section class="py-24 px-4 bg-white overflow-hidden">
  <div class="container mx-auto max-w-6xl">
    <div class="mb-16">
      <h2 class="text-4xl md:text-5xl font-bold tracking-tight mb-4">
        Send, receive, swap.<br />
        All in one place.
      </h2>
    </div>

    <!-- Phone Mockups Row -->
    <div class="flex flex-col md:flex-row justify-center items-end gap-8 md:gap-16 mb-24">
      
      <!-- Phone 1: Send -->
      <div class="flex flex-col items-center">
        <div class="relative w-[280px] h-[560px] bg-black rounded-[40px] border-[8px] border-gray-900 shadow-2xl overflow-hidden mb-6">
          <!-- Screen Content -->
          <div class="w-full h-full bg-black text-white p-6 pt-12 flex flex-col">
            <div class="flex justify-between items-center mb-6">
              <span class="text-xs font-medium">9:41</span>
              <div class="flex gap-1">
                <div class="w-4 h-2.5 bg-white rounded-sm"></div>
              </div>
            </div>
            
            <div class="flex flex-col items-center mt-4">
               <div class="w-16 h-16 bg-gray-800 rounded-full mb-4"></div>
               <div class="text-center mb-8">
                 <div class="text-sm text-gray-400">Known Address</div>
                 <div class="text-xs text-gray-500">You watch this wallet</div>
               </div>
               
               <div class="w-full bg-gray-900 rounded-2xl p-4 mb-4">
                 <div class="text-sm font-bold mb-1">Confirm transaction to Vitalik</div>
               </div>
               
               <div class="w-full flex justify-between text-xs text-gray-400 px-2 mb-2">
                 <span>Collectibles</span>
                 <span>ID Required</span>
               </div>
               
               <div class="w-full bg-gray-900 rounded-2xl p-4 flex items-center gap-3 mb-2">
                 <div class="w-8 h-8 bg-blue-500 rounded-full"></div>
                 <div class="flex-1">
                   <div class="text-sm font-bold">12 DeadFellaz</div>
                   <div class="text-xs text-gray-400">DeadFellaz</div>
                 </div>
               </div>

                <div class="w-full bg-gray-900 rounded-2xl p-4 flex items-center gap-3">
                 <div class="w-8 h-8 bg-purple-500 rounded-full"></div>
                 <div class="flex-1">
                   <div class="text-sm font-bold">Benji Taylor</div>
                   <div class="text-xs text-gray-400">@benjitaylor</div>
                 </div>
               </div>
            </div>
            
            <div class="mt-auto">
               <div class="flex justify-between text-xs text-gray-500 mb-2 px-2">
                 <span>$35.18</span>
                 <span>Normal <span class="text-green-500">●</span></span>
               </div>
               <div class="h-1 bg-white rounded-full w-1/3 mx-auto"></div>
            </div>
          </div>
        </div>
        <div class="flex items-center gap-2 text-blue-500 font-medium">
          <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 19l9 2-9-18-9 18 9-2zm0 0v-8"></path></svg>
          Send
        </div>
      </div>

      <!-- Phone 2: Receive (QR Code) -->
      <div class="flex flex-col items-center relative -top-8">
        <div class="relative w-[280px] h-[560px] bg-black rounded-[40px] border-[8px] border-gray-900 shadow-2xl overflow-hidden mb-6">
           <div class="w-full h-full bg-white flex flex-col items-center justify-center p-8">
             <div class="w-48 h-48 bg-black p-2 rounded-xl mb-8">
               <div class="w-full h-full bg-white grid grid-cols-6 grid-rows-6 gap-0.5">
                 <!-- Mock QR Code -->
                 {#each Array(36) as _, i}
                   <div class={`bg-black ${Math.random() > 0.5 ? 'opacity-100' : 'opacity-0'}`}></div>
                 {/each}
               </div>
             </div>
             <button class="bg-black text-white px-6 py-3 rounded-full text-sm font-bold w-full">Share Address</button>
           </div>
        </div>
        <div class="flex items-center gap-2 text-green-500 font-medium">
          <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path></svg>
          Receive
        </div>
      </div>

      <!-- Phone 3: Swap -->
      <div class="flex flex-col items-center">
        <div class="relative w-[280px] h-[560px] bg-black rounded-[40px] border-[8px] border-gray-900 shadow-2xl overflow-hidden mb-6">
          <div class="w-full h-full bg-black text-white p-6 pt-12 flex flex-col">
             <div class="flex justify-between items-center mb-8">
               <span class="font-bold text-lg">Swap</span>
               <div class="w-6 h-6 bg-gray-800 rounded-full"></div>
             </div>
             
             <div class="bg-gray-900 rounded-2xl p-4 mb-2 flex justify-between items-center">
               <div class="flex items-center gap-2">
                 <div class="w-8 h-8 bg-blue-500 rounded-full"></div>
                 <div class="font-bold">Ethereum</div>
               </div>
               <div class="text-right">
                 <div class="font-bold">1.393 WETH</div>
               </div>
             </div>
             
             <div class="flex justify-center -my-3 relative z-10">
               <div class="w-8 h-8 bg-black border-4 border-black rounded-full flex items-center justify-center">
                 <svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path></svg>
               </div>
             </div>
             
             <div class="bg-gray-900 rounded-2xl p-4 mt-2 mb-8 flex justify-between items-center">
                <div class="flex items-center gap-2">
                 <div class="w-8 h-8 bg-black rounded-full border border-gray-700"></div>
                 <div class="font-bold">USDC</div>
               </div>
               <div class="text-right">
                 <div class="font-bold">2,535.04</div>
               </div>
             </div>
             
             <div class="text-center mb-8">
               <div class="text-5xl font-bold mb-2">$20</div>
               <div class="text-sm text-gray-500">≈ 0.005 ETH <span class="text-gray-700">⇅</span></div>
             </div>
             
             <div class="grid grid-cols-3 gap-4 text-center font-medium text-xl mt-auto mb-8">
               <div>1</div><div>2</div><div>3</div>
               <div>4</div><div>5</div><div>6</div>
               <div>7</div><div>8</div><div>9</div>
               <div>.</div><div>0</div><div>←</div>
             </div>
          </div>
        </div>
        <div class="flex items-center gap-2 text-gray-500 font-medium">
          <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7h12m0 0l-4-4m4 4l-4 4m0 6H4m0 0l4 4m-4-4l4-4"></path></svg>
          Swap
        </div>
      </div>

    </div>

    <!-- Features Text Grid -->
    <div class="grid grid-cols-1 md:grid-cols-2 gap-x-16 gap-y-12">
      
      <div>
        <h3 class="text-blue-500 font-bold mb-2 text-sm">Send & Receive</h3>
        <p class="text-gray-500 leading-relaxed text-sm">
          Flawless essentials. Easily send tokens and collectibles with the fewest taps, or share your wallet address by simply scanning a personalized QR code to receive new assets.
        </p>
      </div>

      <div>
        <h3 class="text-blue-500 font-bold mb-2 text-sm">Decentralized Swaps</h3>
        <p class="text-gray-500 leading-relaxed text-sm">
          Trade thousands of tokens with minimal fees, 24/7. Family ensures optimal prices from various exchanges so you can acquire the tokens you want, whenever you want them.
        </p>
      </div>

      <div>
        <h3 class="text-blue-500 font-bold mb-2 text-sm">Full NFT Support</h3>
        <p class="text-gray-500 leading-relaxed text-sm">
          Experience NFTs in their intended format with our full rich media support. Interact with everything, including video, audio, images, and interactive content. The best collectors manage their collections in Family.
        </p>
      </div>

      <div>
        <h3 class="text-blue-500 font-bold mb-2 text-sm">WalletConnect Enabled</h3>
        <p class="text-gray-500 leading-relaxed text-sm">
          Easily access decentralized apps with WalletConnect in Family. Simply pair your wallet with the built-in scanner, and enjoy seamless connectivity to a range of powerful applications across web3.
        </p>
      </div>

      <div>
        <h3 class="text-blue-500 font-bold mb-2 text-sm">Self-Custody</h3>
        <p class="text-gray-500 leading-relaxed text-sm">
          Family is committed to delivering robust security with flexibility to suit your preferences. The self-custodial wallet prioritizes your control, giving you direct access to your private keys and sensitive data at all times.
        </p>
      </div>

      <div>
        <h3 class="text-blue-500 font-bold mb-2 text-sm">Maximum Privacy</h3>
        <p class="text-gray-500 leading-relaxed text-sm">
          Explore web3 on your own terms, with no compromises on privacy or revealing more than you're comfortable with. Family works with or without an email or phone number, letting you choose the experience that's right for you.
        </p>
      </div>

    </div>
  </div>
</section>
