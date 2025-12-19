<script>
  // No imports needed as we use inline SVGs for specific styling control
</script>

<section class="relative h-[calc(100svh-4rem)] flex flex-col overflow-hidden">
  <!-- Content -->
  <div class="flex-shrink-0 flex flex-col justify-center mx-auto max-w-5xl px-6 sm:px-8 text-center py-12 sm:py-16 md:py-20">
    <h1 class="mb-5 sm:mb-6 text-3xl sm:text-4xl md:text-5xl lg:text-6xl font-serif text-gray-900 leading-[1.1] sm:leading-[0.95] tracking-[-0.01em]">
      Modernize Financial Operations with Confidence
    </h1>
    <p class="mx-auto mb-8 sm:mb-10 max-w-2xl text-base sm:text-lg text-gray-600 leading-relaxed">
      Deploy AI across your organization with guidance that accelerates transformation and ensures regulatory readiness
    </p>

    <div class="flex justify-center">
        <a href="https://calendly.com/jose-altura/30min" target="_blank" rel="noopener noreferrer" class="rounded-full bg-black px-6 sm:px-8 py-3 text-sm sm:text-base font-medium text-white hover:bg-gray-800 transition-all inline-block">
            Schedule Consultation
        </a>
    </div>
  </div>

  <!-- Hero Visual -->
  <div class="relative flex-1 min-h-0 w-full max-w-[1400px] mx-auto px-4 sm:px-8 md:px-12 lg:px-16 pb-4 sm:pb-6">
    <div class="relative w-full h-full overflow-hidden rounded-xl">
      <img
        src="/hero-nyc.jpg"
        alt="New York City Skyline"
        class="absolute inset-0 w-full h-full object-cover object-bottom grayscale"
      />
      <!-- Green tint overlay -->
      <div class="absolute inset-0 bg-primary-900/40 mix-blend-multiply"></div>

      <!-- Main Visual Overlay -->
      <div class="absolute inset-4 sm:inset-6 md:inset-8 flex items-center justify-center animate-fade-in-up">
        <div class="w-full max-w-sm bg-white/95 backdrop-blur-md rounded-2xl shadow-2xl overflow-hidden">
          <!-- Header -->
          <div class="px-5 py-4 flex items-center justify-between">
            <div class="flex items-center gap-3">
              <div class="h-10 w-10 rounded-xl bg-primary-600 flex items-center justify-center text-white">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
              </div>
              <div>
                <div class="text-sm font-semibold text-gray-900">GRC Status</div>
                <div class="text-xs text-gray-500">Real-time</div>
              </div>
            </div>
            <div class="flex items-center gap-1.5">
              <span class="h-2 w-2 rounded-full bg-emerald-500 animate-pulse"></span>
              <span class="text-xs font-medium text-emerald-600">Active</span>
            </div>
          </div>

          <!-- Stats Grid -->
          <div class="px-5 pb-5 grid grid-cols-3 gap-3">
            <div class="text-center py-3 bg-gray-50 rounded-xl">
              <div class="text-xl font-bold text-gray-900">98%</div>
              <div class="text-[10px] uppercase tracking-wider text-gray-500 mt-0.5">Compliant</div>
            </div>
            <div class="text-center py-3 bg-gray-50 rounded-xl">
              <div class="text-xl font-bold text-gray-900">24/7</div>
              <div class="text-[10px] uppercase tracking-wider text-gray-500 mt-0.5">Monitor</div>
            </div>
            <div class="text-center py-3 bg-gray-50 rounded-xl">
              <div class="text-xl font-bold text-gray-900">SOC2</div>
              <div class="text-[10px] uppercase tracking-wider text-gray-500 mt-0.5">Certified</div>
            </div>
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
