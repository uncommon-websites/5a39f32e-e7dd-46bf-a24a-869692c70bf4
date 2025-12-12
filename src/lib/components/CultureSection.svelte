<script lang="ts">
  const cards = [
    {
      title: "11 Years in Venture Capital",
      subtitle: "Insider Knowledge of What Investors Want",
      image: "/generated/image-experienced-venture-capitalist-reviewing-1765565372787-4.webp"
    },
    {
      title: "Battle-Tested Narrative Design",
      subtitle: "Hundreds of Decks, Proven Frameworks",
      image: "/generated/image-close-up-of-hands-sketching-narrative-fl-1765565375194-5.webp"
    },
    {
      title: "$100M+ Raised by Clients",
      subtitle: "From Pre-Seed to Series A Success",
      image: "/generated/image-startup-founder-and-investor-shaking-han-1765565377498-6.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      Most pitch deck consultants have never sat on the other side of the table. I have. With 11 years in venture capital, I know exactly what makes investors say yes—and what makes them pass.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each cards as card}
      <div class="group">
        <div class="aspect-[4/3] overflow-hidden rounded-lg mb-4 bg-gray-100">
          <img src={card.image} alt={card.title} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
        </div>
        <h3 class="text-sm text-gray-500 mb-1">{card.title}</h3>
        <p class="text-sm font-bold">{card.subtitle}</p>
        
        <div class="flex justify-between mt-4 text-xs text-gray-400">
           <span>01</span>
           <span>-></span>
        </div>
      </div>
    {/each}
  </div>
</section>
