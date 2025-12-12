<script lang="ts">
  const projects = [
    {
      client: "FinTech Startup",
      desc: "From scattered ideas to $8M Series A. Crafted narrative that connected regulatory compliance with consumer trust.",
      bg: "bg-black",
      img: "/generated/image-confident-startup-founder-presenting-pit-1765565362958-0.webp",
      dark: true
    },
    {
      client: "HealthTech Platform",
      desc: "Positioned complex medical AI as accessible healthcare solution. Raised $5M seed round.",
      bg: "bg-gray-100",
      img: "/generated/image-healthcare-startup-founder-working-on-la-1765565365854-1.webp",
      dark: false
    },
    {
      client: "B2B SaaS",
      desc: "Transformed technical product into compelling business story. $12M Series A from top-tier VCs.",
      bg: "bg-gray-900",
      img: "/generated/image-b2b-saas-startup-team-collaborating-in-m-1765565368169-2.webp",
      dark: true
    },
    {
      client: "Climate Tech",
      desc: "Bridged science and business narrative. Secured $15M from impact investors and traditional VCs.",
      bg: "bg-[#1a1a1a]",
      img: "/generated/image-young-diverse-startup-team-celebrating-f-1765565370493-3.webp",
      dark: true,
      full: true
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">We transform complex visions into investor-ready narratives</span> that resonate with VCs and secure funding. From pre-seed to Series A, we've helped founders raise hundreds of millions.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each projects as project}
      <div class="group cursor-pointer {project.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${project.bg} mb-4 ${project.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if project.img}
             <img src={project.img} alt={project.client} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Placeholder for logos on solid bg -->
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${project.dark ? 'text-white' : 'text-black'}`}>{project.client}</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{project.client}</h3>
        <p class="text-sm text-gray-600">{project.desc}</p>
      </div>
    {/each}
  </div>
</section>
