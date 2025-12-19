<script>
  import { fly, fade } from 'svelte/transition';
  import { cubicOut, cubicIn } from 'svelte/easing';

  export let active = "Solutions";

  let mobileMenuOpen = false;

  function toggleMenu() {
    mobileMenuOpen = !mobileMenuOpen;
  }

  function closeMenu() {
    mobileMenuOpen = false;
  }
</script>

<header class="sticky top-0 z-50 w-full border-b border-gray-100 bg-white/95 backdrop-blur-sm">
  <div class="mx-auto flex h-16 max-w-7xl items-center justify-between px-4 sm:px-6 lg:px-8">
    <a href="/" class="flex items-center">
      <img src="/altura_logo_black.svg" alt="Altura Labs" class="h-6" />
    </a>

    <!-- Desktop Navigation -->
    <nav class="hidden md:flex items-center gap-8">
      <a href="/#solutions" class="text-sm font-medium text-gray-600 hover:text-gray-900 transition-colors">Solutions</a>
      <a href="/#services" class="text-sm font-medium text-gray-600 hover:text-gray-900 transition-colors">Services</a>
      <a href="/about" class="text-sm font-medium text-gray-600 hover:text-gray-900 transition-colors">About</a>
    </nav>

    <div class="flex items-center gap-4">
      <a href="/contact" class="rounded-full bg-black px-4 sm:px-5 py-2 text-sm font-medium text-white hover:bg-gray-800 transition-colors">
        Contact Us
      </a>

      <!-- Mobile Menu Button -->
      <button
        on:click={toggleMenu}
        class="md:hidden relative w-10 h-10 flex items-center justify-center text-gray-700 hover:text-gray-900 transition-colors"
        aria-label="Toggle menu"
        aria-expanded={mobileMenuOpen}
      >
        <span class="sr-only">Menu</span>
        <div class="w-5 flex flex-col gap-1">
          <span
            class="block h-0.5 w-full bg-current transition-all duration-200 origin-center"
            class:translate-y-[6px]={mobileMenuOpen}
            class:rotate-45={mobileMenuOpen}
          ></span>
          <span
            class="block h-0.5 w-full bg-current transition-all duration-200"
            class:opacity-0={mobileMenuOpen}
          ></span>
          <span
            class="block h-0.5 w-full bg-current transition-all duration-200 origin-center"
            class:-translate-y-[6px]={mobileMenuOpen}
            class:-rotate-45={mobileMenuOpen}
          ></span>
        </div>
      </button>
    </div>
  </div>
</header>

<!-- Full Page Mobile Menu -->
{#if mobileMenuOpen}
  <div
    class="md:hidden fixed inset-0 z-[100] bg-white flex flex-col"
    transition:fade={{ duration: 200 }}
  >
    <!-- Header -->
    <div class="flex h-16 items-center justify-between px-4 border-b border-gray-100">
      <a href="/" on:click={closeMenu} class="flex items-center">
        <img src="/altura_logo_black.svg" alt="Altura Labs" class="h-6" />
      </a>
      <button
        on:click={closeMenu}
        class="w-10 h-10 flex items-center justify-center text-gray-700"
        aria-label="Close menu"
      >
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <line x1="18" y1="6" x2="6" y2="18"></line>
          <line x1="6" y1="6" x2="18" y2="18"></line>
        </svg>
      </button>
    </div>

    <!-- Navigation Links -->
    <nav class="flex-1 flex flex-col justify-center px-8">
      {#each [
        { href: '/#solutions', label: 'Solutions' },
        { href: '/#services', label: 'Services' },
        { href: '/about', label: 'About' },
        { href: '/security', label: 'Security' }
      ] as item, i}
        <a
          href={item.href}
          on:click={closeMenu}
          class="py-4 text-3xl font-serif text-gray-900 hover:text-primary-600 transition-colors"
          in:fly={{ y: 20, duration: 300, delay: 100 + i * 50, easing: cubicOut }}
          out:fly={{ y: -10, duration: 150, easing: cubicIn }}
        >
          {item.label}
        </a>
      {/each}
    </nav>

    <!-- Footer CTA -->
    <div
      class="px-8 pb-12"
      in:fly={{ y: 20, duration: 300, delay: 300, easing: cubicOut }}
      out:fade={{ duration: 100 }}
    >
      <a
        href="/contact"
        on:click={closeMenu}
        class="block w-full rounded-full bg-black px-5 py-4 text-base font-medium text-white text-center hover:bg-gray-800 transition-colors"
      >
        Contact Us
      </a>
    </div>
  </div>
{/if}
