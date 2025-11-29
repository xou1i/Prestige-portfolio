<script>

  import gsap from "gsap";
  import { onMount } from "svelte";
  onMount(() => {
  const tl = gsap.timeline({
    defaults: { duration: 1.0, ease: "power2.out" }
  });

  tl.from(".hero-title", { opacity: 0, y: 20 })
    .from(".hero-subtitle", { opacity: 0, y: 15 }, "-=0.6")
    .from(".hero-tag", { opacity: 0, y: 10 }, "-=0.6")
    .from(".hero-btn", { opacity: 50, y: 15, stagger: 0.15 }, "-=0.5");
});

</script>

<section id="home" class="w-full bg-white pt-32 pb-24">
  <div class="max-w-3xl mx-auto px-6 text-center space-y-6">

    <!-- Title -->
    <h1 class="hero-title text-4xl md:text-5xl font-poppins font-black
            bg-gradient-to-r from-[#011E6C] to-[#1A3FA3]
            bg-clip-text text-transparent">
      Hi, I'm Ghaith
    </h1>

    <!-- Subtitle -->
    <h2 class="hero-subtitle font-poppins font-bold text-lg md:text-xl font-semibold text-gray-700 leading-relaxed">
      Graphic Designer  • UI/UX Designer  • Front-End Developer
    </h2>

    <!-- Tagline -->
    <p class="hero-tag text-gray-400 text-xl max-w-2xl mx-auto"
    style="font-family: 'Sooner', sans-serif;">
      When Design Meets Code !
    </p>

    <!-- Buttons -->
    <div class="flex justify-center gap-4 pt-4 hero-buttons">


      <!-- Hire Me (Orange Gradient + Darker hover) -->
<a href="#contact"
   class="hero-btn px-8 py-3 rounded-full font-poppins font-bold text-white 
               bg-gradient-to-r from-[#FFB74D] to-[#FF9800]
               hover:from-[#F9A825] hover:to-[#EF6C00]
               shadow-md hover:shadow-xl 
               transition duration-300">
  Hire Me
</a>




     <!-- Download CV (Border Blue + Hover Gradient) -->
<!-- Download CV (Smooth Transition) -->
<a href="https://drive.google.com/file/d/1c6dcNWXG0SC2TNHtCoshsPW0JZyEk4ft/view?usp=sharing" 
   target="_blank" 
   class="hero-btn px-8 py-3 rounded-full font-poppins font-bold 
               border-2 border-[#011E6C] text-[#011E6C]
               bg-white
               hover:text-white 
               hover:bg-gradient-to-r hover:from-[#011E6C] hover:to-[#1A3FA3]
               shadow-md hover:shadow-xl 
               transition-all duration-500 ease-[cubic-bezier(0.4,0,0.2,1)]">
  Download CV
</a>





    </div>

  </div>
</section>



