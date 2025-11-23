<script>
  import { onMount } from "svelte";
  import gsap from "gsap";

  onMount(() => {
    gsap.from(".contact-wrapper", {
      opacity: 0,
      duration: 1.5,
      ease: "power2.out",
    });
  });
</script>

<section id="contact" class="contact-wrapper w-full bg-gradient-to-r from-[#001347] to-[#011E6C] py-10 contact-wrapper">
  <div class="max-w-3xl mx-auto px-6 text-center space-y-6">

    <!-- Title -->
    <h2 class="text-4xl md:text-5xl font-poppins font-bold 
               bg-gradient-to-r from-[#FFFFFF] to-[#DFDFDF]
               bg-clip-text text-transparent">
      Contact Me
    </h2>

    <p class="font-poppins font-Medium text-gray-300 text-2xl">Let’s be in touch</p>

    <!-- ICON BUTTONS -->
    <div class="flex items-center justify-center gap-6 pt-8 flex-wrap">

      <!-- EMAIL -->
      <!-- svelte-ignore a11y_consider_explicit_label -->
      <!-- svelte-ignore a11y_missing_attribute -->

      <a href="https://mail.google.com/mail/?view=cm&fs=1&to=des.ghaith@gmail.com"
   target="_blank"
   class="icon-btn w-12 h-12 rounded-full 
          bg-gradient-to-r from-[#FFB74D] to-[#FF9800] 
          flex items-center justify-center
          border-2 border-transparent hover:border-white
          transition-all duration-500 ease-[cubic-bezier(0.16,1,0.3,1)]
          hover:shadow-[0_0_28px_rgba(255,255,255,0.55)]
          hover:cursor-pointer">

  <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-mail-icon lucide-mail"><path d="m22 7-8.991 5.727a2 2 0 0 1-2.009 0L2 7"/><rect x="2" y="4" width="20" height="16" rx="2"/></svg>
</a>

      <!-- GITHUB -->
       <!-- svelte-ignore a11y_consider_explicit_label -->
      <a href="https://github.com/xou1i"
      target="_blank"
        class="icon-btn w-12 h-12 rounded-full 
       bg-gradient-to-r from-[#FFB74D] to-[#FF9800] 
       flex items-center justify-center
       border-2 border-transparent hover:border-white
       transition-all duration-500 ease-[cubic-bezier(0.16,1,0.3,1)]
       hover:shadow-[0_0_28px_rgba(255,255,255,0.55)]">

        <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#ffffff" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-github-icon lucide-github"><path d="M15 22v-4a4.8 4.8 0 0 0-1-3.5c3 0 6-2 6-5.5.08-1.25-.27-2.48-1-3.5.28-1.15.28-2.35 0-3.5 0 0-1 0-3 1.5-2.64-.5-5.36-.5-8 0C6 2 5 2 5 2c-.3 1.15-.3 2.35 0 3.5A5.403 5.403 0 0 0 4 9c0 3.5 3 5.5 6 5.5-.39.49-.68 1.05-.85 1.65-.17.6-.22 1.23-.15 1.85v4"/><path d="M9 18c-4.51 2-5-2-7-2"/></svg>
      </a>

      <!-- LINKEDIN -->
       <!-- svelte-ignore a11y_consider_explicit_label -->
      <a href="https://www.linkedin.com/in/ghaith-284300359/"
      target="_blank"
         class="icon-btn w-12 h-12 rounded-full 
       bg-gradient-to-r from-[#FFB74D] to-[#FF9800] 
       flex items-center justify-center
       border-2 border-transparent hover:border-white
       transition-all duration-500 ease-[cubic-bezier(0.16,1,0.3,1)]
       hover:shadow-[0_0_28px_rgba(255,255,255,0.55)]">

        <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#ffffff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-linkedin-icon lucide-linkedin"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect width="4" height="12" x="2" y="9"/><circle cx="4" cy="4" r="2"/></svg>
      </a>


      <!-- BEHANCE -->
       <!-- svelte-ignore a11y_consider_explicit_label -->
      <a href="https://www.behance.net/prestigedesign2"
      target="_blank"
         class="icon-btn w-12 h-12 rounded-full 
       bg-gradient-to-r from-[#FFB74D] to-[#FF9800] 
       flex items-center justify-center
       border-2 border-transparent hover:border-white
       transition-all duration-500 ease-[cubic-bezier(0.16,1,0.3,1)]
       hover:shadow-[0_0_28px_rgba(255,255,255,0.55)]">

        <svg width="36" height="36" viewBox="0 0 24.00 24.00" fill="none" xmlns="http://www.w3.org/2000/svg" stroke="#ffffff" stroke-width="0.00024000000000000003"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M20.3331 7.66665H14.4999V6H20.3331V7.66665ZM21.7715 15.9999C21.4031 17.0807 20.0806 18.4999 17.5207 18.4999C14.959 18.4999 12.884 17.059 12.884 13.7707C12.884 10.5125 14.8215 8.83747 17.439 8.83747C20.0073 8.83747 21.5756 10.3225 21.9181 12.5258C21.9831 12.9474 22.0089 13.5158 21.9973 14.3091H15.3082C15.4165 16.9849 18.2107 17.069 19.1315 15.9999H21.7715ZM15.3665 12.6666H19.504C19.4165 11.3774 18.5573 10.8174 17.4398 10.8174C16.2182 10.8174 15.5424 11.4574 15.3665 12.6666ZM7.38828 18.4899H2V6.0175H7.7941C12.3574 6.085 12.4441 10.5541 10.0607 11.7724C12.9449 12.8224 13.0415 18.4899 7.38828 18.4899ZM4.49997 10.9999H7.48661C9.57658 10.9999 9.90825 8.49997 7.22661 8.49997H4.49997V10.9999ZM7.32578 13.4999H4.49997V16.0132H7.28411C9.82992 16.0132 9.67408 13.4999 7.32578 13.4999Z" fill="#ffffff"></path> </g></svg>
      </a>

      <!-- INSTAGRAM -->
       <!-- svelte-ignore a11y_consider_explicit_label -->
      <a href="https://www.instagram.com/iq.prestige/"
      target="_blank"
         class="icon-btn w-12 h-12 rounded-full 
       bg-gradient-to-r from-[#FFB74D] to-[#FF9800] 
       flex items-center justify-center
       border-2 border-transparent hover:border-white
       transition-all duration-500 ease-[cubic-bezier(0.16,1,0.3,1)]
       hover:shadow-[0_0_28px_rgba(255,255,255,0.55)]">

        <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#ffffff" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-instagram-icon lucide-instagram"><rect width="20" height="20" x="2" y="2" rx="5" ry="5"/><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/><line x1="17.5" x2="17.51" y1="6.5" y2="6.5"/></svg>
      </a>



      <!-- PHONE — SPECIAL EXPAND -->
       <!-- svelte-ignore a11y_consider_explicit_label -->
      <!-- PHONE — FIXED ICON + EXPAND ON HOVER -->

<a href="tel:+964 775 565 8593"> 
       
<div 
  
  class="relative group flex items-center 
         bg-gradient-to-r from-[#FFB74D] to-[#FF9800]
         rounded-full border-2 border-transparent hover:border-white
         cursor-pointer overflow-hidden
         h-12 w-12 hover:w-56
         transition-all duration-500 ease-[cubic-bezier(0.16,1,0.3,1)]
         hover:shadow-[0_0_28px_rgba(255,255,255,0.55)]">

  <!-- ICON ثابت -->
  <div class="w-12 h-12 flex items-center justify-center flex-shrink-0">
    <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28"
         viewBox="0 0 24 24" fill="none" stroke="#ffffff" stroke-width="2.5"
         stroke-linecap="round" stroke-linejoin="round">
      <path d="M13.832 16.568a1 1 0 0 0 1.213-.303l.355-.465A2 2 0 0 1 17 15h3a2 2 0 0 1 2 2v3a2 2 0 0 1-2 2A18 18 0 0 1 2 4a2 2 0 0 1 2-2h3a2 2 0 0 1 2 2v3a2 2 0 0 1-.8 1.6l-.468.351a1 1 0 0 0-.292 1.233 14 14 0 0 0 6.392 6.384"/>
    </svg>
  </div>

  <!-- Number -->
  <span 
    class="opacity-0 group-hover:opacity-100 
           transition-all duration-500 ease-[cubic-bezier(0.16,1,0.3,1)]
           whitespace-nowrap pl-4 text-white font-semibold text-[15px]">
    +964 775 565 8593
  </span>

</div>
</a>




    </div>

  </div>
</section>
