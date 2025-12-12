<script lang="ts">
  // Trusted by founders and backed by experience
  const logos = [
    "Pre-Seed Founders",
    "Seed Stage Startups",
    "Series A Companies",
    "YC Alumni"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-black via-gray-900 to-white text-white">
  <!-- Gradient overlay/background handling -->
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,#000_0%,#1a1a1a_40%,#666_70%,#fff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight">
      Transform startup fundraising success through battle-tested narrative design. <span class="text-gray-400">11 years of venture capital experience. $100M+ raised by clients. Investor-ready decks that tell your story.</span>
    </h1>
  </div>

  <div class="border-t border-gray-600 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-50 text-sm">
    {#each logos as logo}
      <div class="h-8 flex items-center justify-center font-medium">{logo}</div>
    {/each}
    <div class="h-8 flex items-center justify-center font-medium">Tech Startups</div>
  </div>
</section>
