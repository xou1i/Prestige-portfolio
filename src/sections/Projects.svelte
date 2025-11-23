<script>
  import { onMount } from "svelte";
  import gsap from "gsap";
  import ScrollTrigger from "gsap/ScrollTrigger";

  gsap.registerPlugin(ScrollTrigger);

  onMount(() => {
    const cards = document.querySelectorAll(".project-card");

    cards.forEach((card, index) => {
      gsap.fromTo(
        card,
        { opacity: 0 },   // fade only
        {
          opacity: 1,
          duration: 0.3,
          eese: "power2.out",
          delay: index * 0.2,
          scrollTrigger: {
            trigger: card,
            start: "top 90%",
            toggleActions: "play none none none"
          }
        }
      );
    });
  });
</script>

<section id="projects" class="w-full bg-white py-24">
  <div class="max-w-5xl mx-auto px-6 text-center space-y-10">

    <!-- Title -->
    <h2
      class="text-3xl md:text-4xl font-poppins font-bold  
             bg-gradient-to-r from-[#011E6C] to-[#1A3FA3]
             bg-clip-text text-transparent"
    >
      Projects
    </h2>

    <!-- Description -->
    <p class="font-poppins font-Medium text-gray-600 text-lg leading-relaxed max-w-2xl mx-auto">
      Some of my recent programming and design work.
    </p>

    <!-- Projects Grid -->
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8 pt-6">

      <!-- Project 1 -->
      <div
        class="project-card opacity-0 w-full p-6 rounded-2xl 
               shadow-[0_8px_32px_rgba(0,0,0,0.06)]
               bg-white border border-gray-100 
               hover:shadow-xl hover:-translate-y-2
               transition duration-300 cursor-pointer text-left"
      >
        <h3 class="font-poppins font-semibold text-xl text-[#011E6C] mb-3">Todo App</h3>
        <p class="font-poppins font-Medium text-gray-600 text-sm leading-relaxed">
          A modern task management app built using HTML, Tailwind CSS, and JavaScript.
        </p>
      </div>

      <!-- Project 2 -->
      <div
        class="project-card opacity-0 w-full p-6 rounded-2xl 
               shadow-[0_8px_32px_rgba(0,0,0,0.06)]
               bg-white border border-gray-100 
               hover:shadow-xl hover:-translate-y-2
               transition duration-300 cursor-pointer text-left"
      >
        <h3 class=" font-poppins font-semibold text-xl text-[#011E6C] mb-3">Calculator</h3>
        <p class="font-poppins font-Medium text-gray-600 text-sm leading-relaxed">
          A functional calculator with a clean UI built using HTML, CSS, and JavaScript.
        </p>
      </div>

      <!-- Project 3 -->
      <div
        class="project-card opacity-0 w-full p-6 rounded-2xl 
               shadow-[0_8px_32px_rgba(0,0,0,0.06)]
               bg-white border border-gray-100 
               hover:shadow-xl hover:-translate-y-2
               transition duration-300 cursor-pointer text-left"
      >
        <h3 class="font-poppins font-semibold text-xl text-[#011E6C] mb-3">Design Projects</h3>
        <p class="font-poppins font-Medium text-gray-600 text-sm leading-relaxed">
          Branding, social media visuals, and UI layouts showcased on my Behance profile.
        </p>
      </div>

    </div>

  </div>
</section>
