<script lang="ts">
  let openIndex: number | null = null;

  const faqs = [
    {
      question: "Is Family safe?",
      answer: "Family is a self-custodial wallet, meaning you have full control over your funds and private keys. We never have access to your assets. We also undergo regular security audits to ensure the highest level of protection."
    },
    {
      question: "Can I switch from another wallet?",
      answer: "Yes! You can easily import your existing wallet using your secret recovery phrase. Family supports importing from MetaMask, Rainbow, Coinbase Wallet, and many others."
    },
    {
      question: "What networks does Family support?",
      answer: "Family is built for Ethereum and supports all Ethereum-based networks (L2s) like Optimism, Arbitrum, Base, Polygon, and more."
    }
  ];

  function toggle(index: number) {
    if (openIndex === index) {
      openIndex = null;
    } else {
      openIndex = index;
    }
  }
</script>

<section class="py-24 px-4 bg-white">
  <div class="container mx-auto max-w-6xl flex flex-col md:flex-row gap-16">
    <div class="md:w-1/3">
      <h2 class="text-4xl md:text-5xl font-bold tracking-tight mb-4">Frequently Asked Questions</h2>
    </div>

    <div class="md:w-2/3">
      <div class="space-y-4">
        {#each faqs as faq, i}
          <div class="border-b border-gray-100 pb-4">
            <button 
              class="w-full flex justify-between items-center py-4 text-left font-bold text-lg hover:text-blue-600 transition-colors"
              on:click={() => toggle(i)}
            >
              {faq.question}
              <span class={`transform transition-transform duration-200 ${openIndex === i ? 'rotate-45' : ''} text-orange-500 font-normal text-2xl`}>+</span>
            </button>
            {#if openIndex === i}
              <div class="pb-4 text-gray-500 leading-relaxed">
                {faq.answer}
              </div>
            {/if}
          </div>
        {/each}
      </div>
      
      <div class="mt-8">
        <a href="#" class="text-orange-500 font-bold flex items-center gap-2 hover:gap-3 transition-all">
          See More FAQs 
          <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
        </a>
      </div>
    </div>
  </div>
</section>
