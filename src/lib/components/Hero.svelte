<script>
  // No imports needed as we use inline SVGs for specific styling control
</script>

<section class="relative flex flex-col items-center justify-start pt-20 pb-32 overflow-hidden">
  <!-- Content -->
  <div class="z-10 mx-auto max-w-5xl px-4 text-center mb-16">
    <h1 class="mb-6 text-5xl md:text-6xl lg:text-7xl font-serif text-gray-900 leading-[0.95] tracking-[-0.01em]">
      Modernize Financial Operations with Confidence
    </h1>
    <p class="mx-auto mb-10 max-w-2xl text-lg text-gray-600 leading-relaxed">
      Deploy AI across your organization with guidance that accelerates transformation and ensures regulatory readiness
    </p>

    <div class="flex justify-center">
        <div class="relative group">
            <!-- Decorative brackets/corners could be added here if needed, but simple button for now -->
            <a href="https://calendly.com/jose-altura/30min" target="_blank" rel="noopener noreferrer" class="relative rounded-full bg-black px-8 py-3 text-base font-medium text-white hover:bg-gray-800 transition-all inline-block">
                Schedule Consultation
            </a>
            <!-- Decorative curved corners -->
            <div class="absolute -top-2 -left-2 h-6 w-6 border-t-2 border-l-2 border-black rounded-tl-full"></div>
            <div class="absolute -bottom-2 -right-2 h-6 w-6 border-b-2 border-r-2 border-black rounded-br-full"></div>
        </div>
    </div>
  </div>

  <!-- Hero Image & Search Interface -->
  <div class="relative w-full max-w-7xl mx-auto px-4">
    <div class="relative aspect-[4/3] md:aspect-[16/9] lg:aspect-[21/9] w-full overflow-hidden rounded-lg">
      <img
        src="/hero-nyc.jpg"
        alt="New York City Skyline"
        class="h-full w-full object-cover grayscale"
      />
      <!-- Green tint overlay -->
      <div class="absolute inset-0 bg-primary-900/40 mix-blend-multiply"></div>

      <!-- Overlay Badge -->
      <div class="absolute inset-0 flex items-end md:items-center justify-center p-4 md:p-0 bg-black/10">
        <div class="w-full max-w-xl rounded-xl bg-white p-4 md:p-6 shadow-xl animate-fade-in-up">
            <div class="flex items-center gap-3 md:gap-4 mb-3 md:mb-4">
                <div class="h-10 w-10 md:h-12 md:w-12 flex-shrink-0 rounded-full bg-gradient-to-br from-primary-500 to-primary-700 flex items-center justify-center text-white font-bold">
                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="md:w-6 md:h-6"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/><path d="m9 12 2 2 4-4"/></svg>
                </div>
                <div>
                    <div class="font-semibold text-gray-900 text-sm md:text-base">Technology Modernization with embedded GRC</div>
                    <div class="text-xs md:text-sm text-gray-500">Compliance • Implementation • AI Integration</div>
                </div>
            </div>
            <div class="flex items-center gap-2 text-[10px] md:text-xs text-gray-600">
                <span class="flex items-center gap-1">
                    <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M22 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
                    20+ Years Experience
                </span>
                <span class="text-gray-300">•</span>
                <span>Proven Modernization Roadmaps</span>
            </div>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
    .animate-fade-in-up {
        animation: fadeInUp 0.8s ease-out forwards;
    }
    @keyframes fadeInUp {
        from { opacity: 0; transform: translateY(20px); }
        to { opacity: 1; transform: translateY(0); }
    }
</style>
