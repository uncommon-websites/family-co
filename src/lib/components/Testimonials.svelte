<script>
  // Testimonials
  const testimonials = [
    {
      name: "Daniel Feodoroff",
      handle: "@mrdanielfeo",
      avatar: "https://pbs.twimg.com/profile_images/1508215966453669892/2s_5_2_4_normal.jpg", // Placeholder
      text: "The family app has some of the best UI and UX of a crypto app I've ever seen. Every snippet just blows my mind more and more"
    },
    {
      name: "emm",
      handle: "@web3emm",
      avatar: "https://pbs.twimg.com/profile_images/1605658066453669892/2s_5_2_4_normal.jpg", // Placeholder
      text: "Got in on the @family beta and first impression is THAT THIS is the web2 delightful UI/UX that web3 has been missing"
    },
    {
      name: "skytracker.lens(🌸, 🌿)",
      handle: "@Skytrackr",
      avatar: "https://pbs.twimg.com/profile_images/1605658066453669892/2s_5_2_4_normal.jpg", // Placeholder
      text: "This wallet is absolutely amazing!"
    },
    {
      name: "Adam Waterhouse",
      handle: "@AdamWaterhouse10",
      avatar: "https://pbs.twimg.com/profile_images/1605658066453669892/2s_5_2_4_normal.jpg", // Placeholder
      text: "Love this! The UX around creating a #web3 wallet has needed an overhaul for a long time."
    },
    {
      name: "Zora Zine",
      handle: "@___zine___",
      avatar: "https://pbs.twimg.com/profile_images/1605658066453669892/2s_5_2_4_normal.jpg", // Placeholder
      text: "Best wallet to experience our text NFTs"
    },
    {
      name: "liquid density",
      handle: "@liquiddensity",
      avatar: "https://pbs.twimg.com/profile_images/1605658066453669892/2s_5_2_4_normal.jpg", // Placeholder
      text: "This is absolutely the best wallet from a user perspective. Never seen anything this approachable and easy to use."
    }
  ];
</script>

<section class="py-24 px-4 bg-white overflow-hidden">
  <div class="container mx-auto max-w-6xl mb-12 flex justify-between items-end">
    <div>
      <h2 class="text-4xl md:text-5xl font-bold tracking-tight mb-4">Friends of Family</h2>
      <p class="text-gray-500">See what people are saying.</p>
    </div>
    <a href="#" class="text-sm font-medium flex items-center gap-1 hover:gap-2 transition-all">
      Follow Family 
      <svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
    </a>
  </div>

  <!-- Marquee / Horizontal Scroll -->
  <div class="flex overflow-x-auto pb-8 gap-6 px-4 snap-x snap-mandatory scrollbar-hide">
    {#each testimonials as t}
      <div class="min-w-[350px] bg-gray-50 p-6 rounded-2xl border border-gray-100 snap-center">
        <div class="flex justify-between items-start mb-4">
          <div class="flex items-center gap-3">
            <div class="w-10 h-10 bg-gray-200 rounded-full overflow-hidden">
               <!-- Placeholder avatar -->
               <div class="w-full h-full bg-gradient-to-br from-gray-300 to-gray-400"></div>
            </div>
            <div>
              <div class="font-bold text-sm">{t.name}</div>
              <div class="text-xs text-gray-500">{t.handle}</div>
            </div>
          </div>
          <svg class="w-5 h-5 text-gray-300" viewBox="0 0 24 24" fill="currentColor"><path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/></svg>
        </div>
        <p class="text-gray-600 text-sm leading-relaxed">
          {t.text}
        </p>
      </div>
    {/each}
  </div>
</section>

<style>
  .scrollbar-hide::-webkit-scrollbar {
      display: none;
  }
  .scrollbar-hide {
      -ms-overflow-style: none;
      scrollbar-width: none;
  }
</style>
