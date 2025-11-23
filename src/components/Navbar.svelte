<script>
  let menuOpen = false;
  let closing = false;

  function toggleMenu() {
    if (menuOpen) {
      closing = true;
      setTimeout(() => {
        menuOpen = false;
        closing = false;
      }, 300);
    } else {
      menuOpen = true;
    }
  }

  function closeMenu() {
    closing = true;
    setTimeout(() => {
      menuOpen = false;
      closing = false;
    }, 300);
  }
</script>

<nav class="fixed top-0 left-0 w-full z-50
            bg-white/30 backdrop-blur-2xl
            border-b border-white/60
            shadow-[0_8px_32px_rgba(0,0,0,0.05)]">

  <div class="max-w-7xl mx-auto px-6 h-16 flex items-center justify-between">

    <!-- Logo -->
    <div 
      style="font-family: 'Sooner'"
      class="text-3xl font-bold tracking-wider cursor-pointer text-[#FFB74D]">
      Prestige
    </div>

    <!-- Desktop Links -->
    <ul class="hidden md:flex items-center space-x-4">
      <li><a href="#home"
        class="px-4 py-2 rounded-full border-2 border-[#011E6C] text-[#011E6C] font-Medium hover:bg-[#011E6C] hover:text-white transition-all">Home</a></li>

      <li><a href="#about"
        class="px-4 py-2 rounded-full border-2 border-[#011E6C] text-[#011E6C] font-Medium hover:bg-[#011E6C] hover:text-white transition-all">About</a></li>

      <li><a href="#skills"
        class="px-4 py-2 rounded-full border-2 border-[#011E6C] text-[#011E6C] font-Medium hover:bg-[#011E6C] hover:text-white transition-all">Skills</a></li>

      <li><a href="#projects"
        class="px-4 py-2 rounded-full border-2 border-[#011E6C] text-[#011E6C] font-Medium hover:bg-[#011E6C] hover:text-white transition-all">Projects</a></li>

      <li><a href="#Experience"
        class="px-4 py-2 rounded-full border-2 border-[#011E6C] text-[#011E6C] font-Medium hover:bg-[#011E6C] hover:text-white transition-all">Experience</a></li>

      <li><a href="#contact"
        class="px-4 py-2 rounded-full border-2 border-[#011E6C] text-[#011E6C] font-Medium hover:bg-[#011E6C] hover:text-white transition-all">Contact</a></li>
    </ul>

    <!-- Mobile Menu Button -->
    <button
      class="md:hidden p-3 rounded-lg text-[#011E6C] hover:text-[#1A3FA3] transition"
      on:click={toggleMenu}
    >
      {#if !menuOpen}
        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none"
             viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
          <path stroke-linecap="round" stroke-linejoin="round"
                d="M4 6h16M4 12h16M4 18h16" />
        </svg>
      {:else}
        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none"
             viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
          <path stroke-linecap="round" stroke-linejoin="round"
                d="M6 18L18 6M6 6l12 12" />
        </svg>
      {/if}
    </button>
  </div>
</nav>

<!-- Mobile Menu -->
{#if menuOpen || closing}
  <div 
    class="md:hidden fixed top-16 left-0 w-full
           bg-white/30 backdrop-blur-2xl
           shadow-lg border-b border-white/40
           p-6 space-y-4 z-40
           {menuOpen ? 'animate-menuOpen' : 'animate-menuClose'}"
  >
    <!-- كل لينك يسوي Close -->
    <a href="#home" on:click={closeMenu}
      class="mobile-link">Home</a>

    <a href="#about" on:click={closeMenu}
      class="mobile-link">About</a>

    <a href="#skills" on:click={closeMenu}
      class="mobile-link">Skills</a>

    <a href="#projects" on:click={closeMenu}
      class="mobile-link">Projects</a>

    <a href="#Experience" on:click={closeMenu}
      class="mobile-link">Experience</a>

    <a href="#contact" on:click={closeMenu}
      class="mobile-link">Contact</a>
  </div>
{/if}

<style>
  @keyframes menuOpen {
    0%   { opacity: 0; transform: translateY(-20px); }
    100% { opacity: 1; transform: translateY(0); }
  }

@keyframes menuClose {
  0%   { opacity: 1; transform: translateY(0); }
  100% { opacity: 0; transform: translateY(-20px); }
}

.animate-menuOpen { animation: menuOpen 0.3s ease-out forwards; }
.animate-menuClose {
  animation: menuClose 0.2s cubic-bezier(0.4, 0, 0.2, 1) forwards;
}



  .mobile-link {
    display: block;
    text-lg: 1.125rem;
    color: #011E6C;
    padding: 0.5rem 1rem;
    border: 1px solid #011E6C;
    border-radius: 9999px;
    transition: all .3s;
    font-weight: 500;
  }
  .mobile-link:hover {
    background: #011E6C;
    color: #fff;
  }
</style>
