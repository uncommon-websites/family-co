<script>
  import FeatureSection from './FeatureSection.svelte';
  import PhoneMockup from './PhoneMockup.svelte';
</script>

<!-- NFT Section -->
<FeatureSection
  subtitle="Gimmie"
  title="The best way to experience NFTs."
  description="View NFTs in their ideal intended format. Full rich media support no matter the type, from video and audio, to images and interactive."
  accentColor="text-orange-400"
  features={[
    { label: "Images", icon: "image" },
    { label: "Video", icon: "video" },
    { label: "3D Models", icon: "box" },
    { label: "Audio", icon: "music" },
    { label: "Interactive Models", icon: "mouse-pointer" },
    { label: "AR Models", icon: "camera" }
  ]}
>
  <div slot="media">
    <PhoneMockup screenClass="bg-gray-100 flex flex-col">
       <div class="p-6 pt-12 flex-1 flex flex-col">
         <div class="flex justify-between items-center mb-4">
           <span class="text-xs font-medium">9:41</span>
         </div>
         
         <div class="bg-white rounded-2xl overflow-hidden shadow-sm mb-4 flex-1 relative">
           <!-- NFT Art Placeholder -->
           <div class="absolute inset-0 bg-gradient-to-br from-blue-400 via-purple-400 to-pink-400">
             <div class="w-full h-full opacity-50" style="background-image: repeating-linear-gradient(90deg, transparent, transparent 20px, rgba(255,255,255,0.2) 20px, rgba(255,255,255,0.2) 40px);"></div>
           </div>
         </div>
         
         <div class="mb-4">
           <h3 class="font-bold text-xl">Spent</h3>
           <p class="text-gray-500 text-sm">Ben Crague • Spent</p>
         </div>
       </div>
    </PhoneMockup>
  </div>
  
  <div slot="extra" class="mt-8">
     <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-2xl border border-gray-100 max-w-sm">
        <div class="w-10 h-10 bg-gray-200 rounded-lg"></div>
        <div>
          <div class="font-bold text-sm">Manage your collectibles</div>
          <div class="text-xs text-gray-500">Hide, Unhide, Order</div>
        </div>
     </div>
  </div>
</FeatureSection>

<!-- Watch Wallets Section -->
<FeatureSection
  reverse={true}
  subtitle="Simple"
  title="Watch the wallets you care about."
  description="Keep up to date with unlimited wallets in view only mode by entering an address or ENS name, and get real-time notifications on any new activity."
  accentColor="text-green-500"
  features={[
    "Watch Any Wallet",
    "Rich Notifications",
    "Fully Customizable"
  ]}
>
  <div slot="media">
    <PhoneMockup screenClass="bg-white flex flex-col">
       <div class="p-6 pt-12">
         <div class="flex justify-between items-center mb-6">
           <div class="w-8 h-8 bg-gray-200 rounded-full"></div>
           <div class="font-bold">Vitalik</div>
           <div class="w-8 h-8"></div>
         </div>
         
         <div class="space-y-4">
           <div class="flex items-center gap-3 p-3 bg-gray-50 rounded-xl">
             <div class="w-10 h-10 bg-orange-100 rounded-full flex items-center justify-center text-orange-500">🦊</div>
             <div class="flex-1">
               <div class="font-bold text-sm">Metamask (Main)</div>
               <div class="text-xs text-gray-500">0x71C...976F</div>
             </div>
             <div class="font-bold text-sm">$2,534</div>
           </div>
           
           <div class="flex items-center gap-3 p-3 bg-gray-50 rounded-xl">
             <div class="w-10 h-10 bg-blue-100 rounded-full flex items-center justify-center text-blue-500">R</div>
             <div class="flex-1">
               <div class="font-bold text-sm">Rainbow (Old)</div>
               <div class="text-xs text-gray-500">vitalik.eth</div>
             </div>
             <div class="font-bold text-sm">$4,509.54</div>
           </div>

           <div class="flex items-center gap-3 p-3 bg-gray-50 rounded-xl">
             <div class="w-10 h-10 bg-green-100 rounded-full flex items-center justify-center text-green-500">T</div>
             <div class="flex-1">
               <div class="font-bold text-sm">Tornado Cash...</div>
               <div class="text-xs text-gray-500">0x123...456</div>
             </div>
             <div class="font-bold text-sm">$120,394</div>
           </div>
         </div>
       </div>
    </PhoneMockup>
  </div>
  
  <div slot="extra" class="mt-8">
     <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-2xl border border-gray-100 max-w-sm">
        <div class="w-10 h-10 bg-gray-200 rounded-lg"></div>
        <div>
          <div class="font-bold text-sm">Watching Wallets</div>
          <div class="text-xs text-gray-500">Real-time alerts</div>
        </div>
     </div>
  </div>
</FeatureSection>

<!-- Activity Section -->
<FeatureSection
  subtitle="Understandable"
  title="Wallet activity you can understand."
  description="Your transactions and wallet history is readable at a glance. No more having to decipher what confusing events with weird names mean. We do that for you."
  accentColor="text-red-500"
  features={[
    "Human-Readable Activity",
    "Real-Time Monitoring",
    "Custom Filtering"
  ]}
>
  <div slot="media">
    <PhoneMockup screenClass="bg-white flex flex-col">
       <div class="p-6 pt-12">
         <div class="flex items-center gap-3 mb-8">
           <div class="w-10 h-10 bg-gray-200 rounded-full"></div>
           <div class="font-bold">Benji Taylor</div>
         </div>
         
         <div class="space-y-6 relative">
            <div class="absolute left-[19px] top-4 bottom-0 w-0.5 bg-gray-100"></div>

            <div class="flex gap-4 relative z-10">
              <div class="w-10 h-10 bg-white border-2 border-gray-100 rounded-full flex items-center justify-center text-xs">⏳</div>
              <div class="flex-1">
                <div class="flex justify-between">
                  <span class="font-bold text-sm">Pending</span>
                  <span class="text-xs text-gray-400">10:42 AM</span>
                </div>
                <div class="text-xs text-gray-500">Sending 1.5 ETH to Vitalik</div>
              </div>
            </div>

            <div class="flex gap-4 relative z-10">
              <div class="w-10 h-10 bg-blue-500 text-white rounded-full flex items-center justify-center text-xs">S</div>
              <div class="flex-1">
                <div class="flex justify-between">
                  <span class="font-bold text-sm">Swap</span>
                  <span class="text-xs text-gray-400">Yesterday</span>
                </div>
                <div class="text-xs text-gray-500">Swapped 100 USDC for ETH</div>
              </div>
            </div>

            <div class="flex gap-4 relative z-10">
              <div class="w-10 h-10 bg-purple-500 text-white rounded-full flex items-center justify-center text-xs">M</div>
              <div class="flex-1">
                <div class="flex justify-between">
                  <span class="font-bold text-sm">Mint</span>
                  <span class="text-xs text-gray-400">Oct 24</span>
                </div>
                <div class="text-xs text-gray-500">Minted DeadFellaz #1029</div>
              </div>
            </div>
         </div>
       </div>
    </PhoneMockup>
  </div>
  
  <div slot="extra" class="mt-8">
     <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-2xl border border-gray-100 max-w-sm">
        <div class="w-10 h-10 bg-gray-200 rounded-lg"></div>
        <div>
          <div class="font-bold text-sm">Wallet Activity</div>
          <div class="text-xs text-gray-500">Made to be better</div>
        </div>
     </div>
  </div>
</FeatureSection>

<!-- Security Section -->
<FeatureSection
  reverse={true}
  subtitle="Secure"
  title="Relentless protection. Restful ease."
  description="Family is fully self-custodial, meaning only you have access to your wallet and its private keys. We have no control over your crypto, nor do we want any."
  accentColor="text-blue-500"
  features={[
    "Self-Custody",
    "Own Your Keys",
    "No Name Required",
    "No Lock-In",
    "Fully Audited"
  ]}
>
  <div slot="media" class="relative">
    <!-- Blue Character Illustration Placeholder -->
    <div class="w-64 h-64 bg-blue-400 rounded-3xl rotate-3 flex items-center justify-center relative">
       <!-- Face -->
       <div class="w-16 h-4 bg-black rounded-full absolute top-1/3 left-1/4"></div> <!-- Eye L -->
       <div class="w-16 h-4 bg-black rounded-full absolute top-1/3 right-1/4"></div> <!-- Eye R -->
       <div class="w-8 h-4 bg-black rounded-b-full absolute top-1/2 left-1/2 -translate-x-1/2"></div> <!-- Mouth -->
       
       <!-- Floating elements around -->
       <div class="absolute -top-10 -left-10 w-12 h-12 bg-blue-200 rounded-full animate-bounce"></div>
       <div class="absolute -bottom-5 -right-10 w-16 h-16 bg-blue-300 rounded-full animate-pulse"></div>
    </div>
  </div>
</FeatureSection>
