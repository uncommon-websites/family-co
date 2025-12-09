<script lang="ts">
  export let reverse: boolean = false;
  export let title: string = "";
  export let subtitle: string = "";
  export let description: string = "";
  export let features: (string | { icon: string, label: string })[] = []; 
  export let accentColor: string = "text-orange-400"; // For the subtitle
</script>

<section class="py-24 px-4 overflow-hidden">
  <div class="container mx-auto max-w-6xl">
    <div class={`flex flex-col md:flex-row items-center gap-16 ${reverse ? 'md:flex-row-reverse' : ''}`}>
      
      <!-- Media Side -->
      <div class="w-full md:w-1/2 flex justify-center">
        <slot name="media" />
      </div>

      <!-- Text Side -->
      <div class="w-full md:w-1/2">
        {#if subtitle}
          <div class={`text-sm font-bold mb-4 uppercase tracking-wide ${accentColor}`}>{subtitle}</div>
        {/if}
        
        <h2 class="text-4xl md:text-5xl font-bold tracking-tight mb-6 leading-tight">{title}</h2>
        
        <p class="text-gray-500 text-lg leading-relaxed mb-10">
          {description}
        </p>

        {#if features.length > 0}
          <div class="grid grid-cols-2 gap-y-4 gap-x-8">
            {#each features as feature}
              <div class="flex items-center gap-3 text-sm font-medium text-gray-600">
                {#if typeof feature === 'string'}
                   <div class={`w-4 h-4 rounded-full border flex items-center justify-center ${accentColor.replace('text-', 'border-')}`}>
                     <svg class={`w-2.5 h-2.5 ${accentColor}`} fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg>
                   </div>
                   {feature}
                {:else}
                   <!-- Custom icon support if needed -->
                   <span>{feature.label}</span>
                {/if}
              </div>
            {/each}
          </div>
        {/if}

        <slot name="extra" />
      </div>

    </div>
  </div>
</section>
