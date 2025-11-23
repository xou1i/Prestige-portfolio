<script>
  import gsap from "gsap";
  import { ScrollTrigger } from "gsap/ScrollTrigger";
  import { onMount } from "svelte";

  gsap.registerPlugin(ScrollTrigger);

  onMount(() => {

  // Title animation
  gsap.from(".about-title", {
    scrollTrigger: {
      trigger: ".about-title",
      start: "top 85%",    // يبدأ قبل الوصول
    },
    opacity: 0,
    y: 20,
    duration: 0.8,
    ease: "power2.out"
  });

  // Description animation
  gsap.from(".about-desc", {
    scrollTrigger: {
      trigger: ".about-desc",
      start: "top 85%",
    },
    opacity: 0,
    y: 20,
    duration: 0.9,
    ease: "power2.out"
  });

  // Cards animation (stagger)
  gsap.from(".about-card", {
    scrollTrigger: {
      trigger: ".about-cards",
      start: "top 80%",
    },
    opacity: 100,
    y: 0,
    duration: 1,
    stagger: 0.15,
    ease: "power2.out"
  });

});
</script>

  

<section id="about" class="w-full bg-white py-24">
  <div class="max-w-4xl mx-auto px-6 text-center space-y-10">

    <!-- Title -->
    <h2 class="about-title text-3xl md:text-4xl font-poppins font-bold 
               bg-gradient-to-r from-[#011E6C] to-[#1A3FA3]
               bg-clip-text text-transparent">
      About Me
    </h2>

    <!-- Description -->
    <p class="about-desc font-poppins font-Medium text-gray-600 text-lg leading-relaxed max-w-2xl mx-auto">
      A second-year Cybersecurity Engineering student who combines 
      visual design with modern front-end development to build clean and 
      meaningful digital experiences.
    </p>

    <!-- Cards -->
    <div class="grid grid-cols-1 md:grid-cols-2 gap-6 pt-6">

      <!-- Card 1 -->
      <div class="about-card p-6 rounded-2xl shadow-[0_8px_32px_rgba(0,0,0,0.06)] 
                  bg-white border border-gray-100 hover:shadow-xl 
                  transition duration-300">
        <h3 class="text-xl font-poppins font-bold text-[#011E6C] mb-2">
          Who Am I?
        </h3>
        <p class="font-poppins font-Medium text-gray-600 text-left">
          A creative thinker who loves mixing design, technology, and 
          modern front-end techniques to craft expressive digital visuals.
        </p>
      </div>

      <!-- Card 2 -->
      <div class="about-card p-6 rounded-2xl shadow-[0_8px_32px_rgba(0,0,0,0.06)] 
                  bg-white border border-gray-100 hover:shadow-xl 
                  transition duration-300">
        <h3 class="text-xl font-poppins font-bold text-[#011E6C] mb-2">
          What I Do?
        </h3>
        <p class="font-poppins font-Medium text-gray-600 text-left">
          I design clean interfaces, craft engaging visuals, and build 
          modern, responsive, user-friendly websites.
        </p>
      </div>

    </div>

  </div>
</section>
