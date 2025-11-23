<script>
  import gsap from "gsap";
  import { onMount } from "svelte";

  onMount(() => {
    // Fade for the whole section
    gsap.from(".exp-wrapper", {
      opacity: 0,
      duration: 1.2,
      ease: "power2.out",
    });

    // Fade + tiny slide for each card
    gsap.from(".exp-item", {
      opacity: 100,
      y: 8,            // VERY slight slide
      duration: 5.0,
      delay: 0.3,
      ease: "power2.out",
      stagger: 0.12,   // items appear one-by-one smoothly
    });
  });
</script>

<section id="Experience" class="exp-wrapper w-full bg-white py-24">
  <div class="max-w-5xl mx-auto px-6 space-y-10">

    <!-- Title -->
    <div class="text-center space-y-4">
      <h2
        class="text-3xl md:text-4xl font-poppins font-bold
               bg-gradient-to-r from-[#011E6C] to-[#1A3FA3]
               bg-clip-text text-transparent"
      >
        Experience
      </h2>

      <p class="font-poppins font-Medium text-gray-600 text-lg">
        A quick look at my design and programming journey.
      </p>
    </div>

    <!-- Cards Wrapper -->
    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">

   <!-- Design Experience Card -->
<div class="exp-item rounded-3xl border-2 border-[#FFB74D] bg-white 
            p-6 md:p-8 
            shadow-[0_8px_25px_rgba(0,0,0,0.15)]
            transition-all duration-300 
            hover:shadow-[0_12px_35px_rgba(0,0,0,0.25)]
            hover:-translate-y-1">

  <div class="space-y-5">

    <h3 class="font-poppins font-semibold text-xl md:text-2xl text-[#FFB74D]">
      Design Experience
    </h3>

    <p class="font-poppins font-Medium text-gray-600 text-sm md:text-base leading-relaxed">
      Focusing on branding, social media visuals, and digital content for different clients.
    </p>

    <!-- Item 1 -->
    <div class="space-y-1">
      <p class="font-poppins font-semibold text-[#011E6C]">
        Freelance Designer <span class="font-poppins font-light text-gray-500 text-xs">(2025 – Present)</span>
      </p>
      <p class="font-poppins font-Medium text-gray-600">Brand identities, social posts, and custom visuals for clients.</p>
    </div>

    <!-- Item 2 -->
    <div class="space-y-1">
      <p class="font-poppins font-semibold text-[#011E6C]">
        Mamame Co. <span class="font-poppins font-light text-gray-500 text-xs">(Jul 2025 – Oct 2025)</span>
      </p>
      <p class="font-poppins font-Medium text-gray-600">Social Media Designs, UI Designs.</p>
    </div>

  </div>

</div>




    <!-- Programming Experience Card -->
<div class="exp-item rounded-3xl border-2 border-[#011E6C] bg-white 
            p-6 md:p-8 
            shadow-[0_8px_25px_rgba(0,0,0,0.15)]
            transition-all duration-300 
            hover:shadow-[0_12px_35px_rgba(0,0,0,0.25)]
            hover:-translate-y-1">

  <div class="space-y-5">

    <h3 class="font-poppins font-semibold text-xl md:text-2xl text-[#011E6C]">
      Programming Journey
    </h3>

    <p class="font-poppins font-Medium text-gray-600 text-sm md:text-base leading-relaxed">
      Learning to build clean user interfaces while studying Cybersecurity Engineering.
    </p>

    <!-- Item 1 -->
    <div class="space-y-1">
      <p class="font-poppins font-semibold text-[#011E6C]">Core Stack</p>
      <p class="font-poppins font-Medium text-gray-600">HTML, Tailwind CSS, JavaScript basics, and Svelte components.</p>
    </div>

    <!-- Item 2 -->
    <div class="space-y-1">
      <p class="font-poppins font-semibold text-[#011E6C]">Projects</p>
      <p class="font-poppins font-Medium text-gray-600">Todo App, Calculator, and Prestige portfolio.</p>
    </div>

    <!-- Item 3 -->
    <div class="space-y-1">
      <p class="font-poppins font-semibold text-[#011E6C]">Education</p>
      <p class="font-poppins font-Medium text-gray-600">Cybersecurity Engineering (Sophomore) at Ashur University.</p>
    </div>

  </div>

</div>




    </div>

  </div>
</section>
