<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
</script>

<main class="min-h-screen bg-white font-sans text-gray-900 selection:bg-gray-900 selection:text-white">
    <Header />

    <section class="py-12 sm:py-16 md:py-32">
        <div class="mx-auto max-w-4xl px-4 sm:px-6 lg:px-8">
            <div class="mb-12">
                <span class="text-[10px] font-mono uppercase tracking-widest text-gray-500">About Altura Labs</span>
            </div>

            <div class="space-y-12 text-2xl md:text-3xl lg:text-4xl font-serif text-gray-900 leading-[1.4] tracking-[-0.01em]">
                <p>
                    Every bank CTO knows that sinking feeling. Another compliance deadline looms. Another system that won't talk to the others. Another consultant who presents the perfect strategy, then disappears before anything actually works.
                </p>

                <p>
                    Financial modernization keeps stalling out. That new fraud detection system still requires manual CSV uploads. The compliance dashboard that took eighteen months doesn't connect to your core banking platform.
                </p>

                <p class="text-gray-500">
                    Meanwhile, competitors launch AI features while you're still copying data between spreadsheets.
                </p>

                <p>
                    Altura recognized what was missing. Banks needed builders who understood both worlds—the rigid requirements of compliance and the fluid possibilities of AI. Partners who could navigate regulations while actually shipping code.
                </p>

                <p>
                    <span class="text-primary-700">Altura translates between what banks have and what they need.</span> Our AI agents handle the mind-numbing compliance checks. Our experts untangle decades of system dependencies. Together, we turn regulatory chaos into clarity.
                </p>

                <p>
                    Because when compliance runs itself, CTOs can finally build the future their customers deserve.
                </p>
            </div>

            <div class="mt-20 pt-12 border-t border-gray-100">
                <div class="flex items-center gap-4">
                    <div class="h-14 w-14 rounded-full bg-gray-900 flex items-center justify-center text-white font-medium text-lg">
                        JG
                    </div>
                    <div>
                        <div class="font-medium text-gray-900">José Abraham García</div>
                        <div class="text-sm text-gray-500">Founder & Managing Director</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <Footer />
</main>
