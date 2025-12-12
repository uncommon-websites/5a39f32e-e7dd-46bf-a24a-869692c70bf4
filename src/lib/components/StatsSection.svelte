<script lang="ts">
  const stats = [
    {
      label: "11 Years in VC",
      desc: "Over a decade working in venture capital, evaluating hundreds of pitch decks and understanding what makes investors say yes. This insider perspective informs every deck I create, ensuring your narrative resonates with the people who matter most.",
      img: "/generated/image-experienced-venture-capitalist-reviewing-1765565372787-4.webp"
    },
    {
      label: "$100M+ Raised",
      desc: "Clients have collectively raised hundreds of millions of dollars across pre-seed, seed, and Series A rounds. From fintech to healthtech to climate tech, proven track record of helping founders secure the funding they need to scale.",
      img: "/generated/image-young-diverse-startup-team-celebrating-f-1765565370493-3.webp"
    },
    {
      label: "Hundreds of Decks",
      desc: "Worked on hundreds of pitch decks throughout my career, from early-stage concepts to growth-stage refinements. Each project deepens my understanding of what works—and what doesn't—when it comes to fundraising narratives.",
      img: "/generated/image-stack-of-pitch-deck-slides-and-business--1765565382059-8.webp"
    },
    {
      label: "Pre-Seed to Series A",
      desc: "Specializing in the critical early stages of fundraising when narrative and positioning matter most. Whether you're raising your first $500K or your Series A, I help you craft the story that gets you to the next milestone.",
      img: "/generated/image-confident-startup-founder-presenting-pit-1765565362958-0.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Numbers tell part of the story. Here's what sets Pitch Partners apart in the crowded world of pitch deck consulting.
    </p>
  </div>

  <div class="space-y-16">
    {#each stats as stat}
      <div class="flex flex-col md:flex-row md:items-start justify-between gap-8 border-b border-gray-100 pb-16 last:border-0">
        <h3 class="text-2xl md:text-4xl font-medium w-full md:w-1/3">{stat.label}</h3>
        <div class="w-full md:w-1/3">
           <p class="text-xs leading-relaxed text-gray-500">{stat.desc}</p>
        </div>
        <div class="w-full md:w-1/6 flex justify-end">
           <img src={stat.img} alt={stat.label} class="w-20 h-20 object-cover rounded bg-gray-100" />
        </div>
      </div>
    {/each}
  </div>
</section>
