<script>
  import gsap from "gsap";
  import { ScrollTrigger } from "gsap/ScrollTrigger";
  import { onMount } from "svelte";

  gsap.registerPlugin(ScrollTrigger);

  onMount(() => {

    // Title
    gsap.from(".skills-title", {
      scrollTrigger: {
        trigger: ".skills-title",
        start: "top 85%",
      },
      opacity: 0,
      y: 20,
      duration: 1,
      ease: "power2.out"
    });

    // Description
    gsap.from(".skills-desc", {
      scrollTrigger: {
        trigger: ".skills-desc",
        start: "top 85%",
      },
      opacity: 0,
      y: 20,
      duration: 1,
      ease: "power2.out"
    });

    // Cards
    gsap.from(".skills-card", {
      scrollTrigger: {
        trigger: ".skills-card",
        start: "top 85%",
      },
      opacity: 100,
      y: 0,
      duration: 1.1,
      stagger: 0.2,
      ease: "power2.out"
    });

    // Skill items
    gsap.from(".skill-item", {
      scrollTrigger: {
        trigger: ".skills-card",
        start: "top 85%",
      },
      opacity: 100,
      y: 0,
      duration: 0.8,
      stagger: 0.08,
      ease: "power2.out"
    });

  });
</script>

<section id="skills" class="w-full bg-white py-24">
  <div class="max-w-4xl mx-auto px-6 text-center space-y-10">

    <!-- Title -->
    <h2 class="skills-title text-3xl md:text-4xl font-poppins font-bold 
               bg-gradient-to-r from-[#011E6C] to-[#1A3FA3]
               bg-clip-text text-transparent">
      Skills
    </h2>

    <!-- Description -->
    <p class="skills-desc font-poppins font-Medium text-gray-600 text-lg leading-relaxed max-w-2xl mx-auto">
      Technologies and tools I use to design and build modern, elegant digital experiences.
    </p>

    <!-- Skills Groups -->
    <div class="grid grid-cols-1 md:grid-cols-2 gap-8 pt-6 justify-center items-center
    hover:cursor-pointer">

      <!-- Programming Skills -->
      <div class="skills-card mx-auto p-6 rounded-2xl shadow-[0_8px_32px_rgba(0,0,0,0.06)] 
                  bg-white border border-gray-100 transition duration-300">
        <h3 class="text-xl font-poppins font-semibold text-[#011E6C] mb-4">
          Programming Skills
        </h3>

        <div class="flex flex-wrap gap-3 justify-center">
          <span class="skill-item px-4 py-2 rounded-full text-sm font-poppins font-semibold 
                       border-2 border-[#011E6C] text-[#011E6C]
                       hover:bg-[#011E6C] hover:text-white
                       transition duration-300">
            HTML
          </span>

          <span class="skill-item px-4 py-2 rounded-full text-sm font-poppins font-semibold  
                       border-2 border-[#011E6C] text-[#011E6C]
                       hover:bg-[#011E6C] hover:text-white
                       transition duration-300">
            Tailwind CSS
          </span>

          <span class="skill-item px-4 py-2 rounded-full text-sm font-poppins font-semibold  
                       border-2 border-[#011E6C] text-[#011E6C]
                       hover:bg-[#011E6C] hover:text-white
                       transition duration-300">
            JS (Svelte)
          </span>
        </div>
      </div>

      <!-- Design Skills -->
      <div class="skills-card mx-auto p-6 rounded-2xl shadow-[0_8px_32px_rgba(0,0,0,0.06)] 
                  bg-white border border-gray-100 transition duration-300">
        <h3 class="text-xl font-poppins font-bold text-[#011E6C] mb-4">
          Design Skills
        </h3>

        <div class="flex flex-wrap gap-3 justify-center">

          <span class="skill-item px-4 py-2 rounded-full text-sm font-poppins font-semibold
                       border-2 border-[#FFB74D] text-[#FFB74D]
                       hover:bg-[#FFB74D] hover:text-white
                       transition duration-300">
            Photoshop
          </span>

          <span class="skill-item px-4 py-2 rounded-full text-sm font-poppins font-semibold 
                       border-2 border-[#FFB74D] text-[#FFB74D]
                       hover:bg-[#FFB74D] hover:text-white
                       transition duration-300">
            Illustrator
          </span>

          <span class="skill-item px-4 py-2 rounded-full text-sm font-poppins font-semibold 
                       border-2 border-[#FFB74D] text-[#FFB74D]
                       hover:bg-[#FFB74D] hover:text-white
                       transition duration-300">
            Figma
          </span>

        </div>
      </div>

    </div>

  </div>
</section>
