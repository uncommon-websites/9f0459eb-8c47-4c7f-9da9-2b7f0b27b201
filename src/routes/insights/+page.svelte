<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
    const insights = [
        {
            category: 'GRC',
            title: 'Why Most GRC Modernization Projects Fail',
            excerpt: 'The three critical mistakes that derail transformation initiatives—and how to avoid them.',
            date: 'Coming Soon'
        },
        {
            category: 'AI',
            title: 'Building AI That Regulators Trust',
            excerpt: 'A framework for implementing explainable AI in regulated financial services.',
            date: 'Coming Soon'
        },
        {
            category: 'Compliance',
            title: 'The True Cost of Manual Compliance',
            excerpt: 'Calculating the hidden expenses of spreadsheet-based compliance workflows.',
            date: 'Coming Soon'
        }
    ];
</script>

<main class="min-h-screen bg-white font-sans text-gray-900 selection:bg-gray-900 selection:text-white">
    <Header />

    <section class="py-12 sm:py-16 md:py-32">
        <div class="mx-auto max-w-4xl px-4 sm:px-6 lg:px-8">
            <div class="mb-12">
                <span class="text-[10px] font-mono uppercase tracking-widest text-gray-500">Resources</span>
            </div>

            <h1 class="text-4xl md:text-5xl lg:text-6xl font-serif text-gray-900 leading-[0.95] tracking-[-0.01em] mb-8">
                Insights
            </h1>

            <p class="text-xl text-gray-500 mb-16 max-w-2xl">
                Perspectives on GRC modernization, AI implementation, and regulatory compliance in financial services.
            </p>

            <!-- Insights Grid -->
            <div class="space-y-8">
                {#each insights as insight}
                    <article class="group border-b border-gray-100 pb-8">
                        <div class="flex flex-col md:flex-row md:items-start md:justify-between gap-4">
                            <div class="flex-1">
                                <span class="text-[10px] font-mono uppercase tracking-widest text-primary-600 mb-3 block">{insight.category}</span>
                                <h2 class="text-2xl font-serif text-gray-900 mb-3 group-hover:text-primary-700 transition-colors">
                                    {insight.title}
                                </h2>
                                <p class="text-gray-500">{insight.excerpt}</p>
                            </div>
                            <div class="flex-shrink-0">
                                <span class="text-xs text-gray-400">{insight.date}</span>
                            </div>
                        </div>
                    </article>
                {/each}
            </div>

        </div>
    </section>

    <Footer />
</main>
