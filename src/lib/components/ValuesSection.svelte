<script lang="ts">
  const photos = [
    {
      title: "Hands-On Collaboration",
      desc: "Every deck is a partnership. I work directly with founders to understand their vision and translate it into compelling narratives that investors can't ignore.",
      img: "/generated/image-one-on-one-consultation-session-between--1765565384417-9.webp"
    },
    {
      title: "Iterative Refinement",
      desc: "Great decks aren't built in a day. Through multiple rounds of feedback and refinement, we polish every slide until your story shines.",
      img: "/generated/image-laptop-screen-showing-pitch-deck-being-r-1765565386715-10.webp"
    },
    {
      title: "Investor-Ready Results",
      desc: "The goal isn't just a pretty deck—it's a fundraising tool that opens doors, starts conversations, and closes rounds.",
      img: "/generated/image-stack-of-pitch-deck-slides-and-business--1765565382059-8.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">How we work together.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      Creating a winning pitch deck is a collaborative process. From initial consultation to final delivery, I'm with you every step of the way, bringing VC expertise and narrative design skills to transform your vision into investor-ready reality.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each photos as photo}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={photo.img} alt={photo.title} class="w-full h-full object-cover" />
        </div>
        <h4 class="text-xs font-bold mb-1">{photo.title}</h4>
        <p class="text-[10px] text-gray-500 leading-relaxed">{photo.desc}</p>
      </div>
    {/each}
  </div>
</section>
