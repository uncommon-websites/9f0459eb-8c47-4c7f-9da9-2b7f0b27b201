<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import { Map, ShieldCheck, Eye, Scale, GitBranch, FileCheck } from 'lucide-svelte';
</script>

<main class="min-h-screen bg-white font-sans text-gray-900 selection:bg-gray-900 selection:text-white">
    <Header />

    <section class="py-12 sm:py-16 md:py-32">
        <div class="mx-auto max-w-4xl px-4 sm:px-6 lg:px-8">
            <div class="mb-12">
                <span class="text-[10px] font-mono uppercase tracking-widest text-gray-500">Services</span>
            </div>

            <h1 class="text-4xl md:text-5xl lg:text-6xl font-serif text-gray-900 leading-[0.95] tracking-[-0.01em] mb-16">
                AI Implementation
            </h1>

            <div class="space-y-12 text-xl md:text-2xl font-serif text-gray-900 leading-[1.4] tracking-[-0.01em]">
                <p>
                    Financial institutions are racing to deploy AI, but most implementations fail. Not because the technology doesn't work—but because it wasn't built with compliance in mind from day one.
                </p>

                <p class="text-gray-500">
                    AI in regulated environments requires a different approach. Model governance, explainability, bias monitoring—these aren't afterthoughts.
                </p>

                <p>
                    <span class="text-primary-700">We build AI solutions that regulators trust</span> because we embed compliance into every layer of the implementation.
                </p>
            </div>

            <!-- What We Deliver -->
            <div class="mt-20 pt-12 border-t border-gray-100">
                <h2 class="text-2xl font-serif text-gray-900 mb-10">What We Deliver</h2>

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Map size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">AI Strategy</h3>
                        <p class="text-sm text-gray-500">Roadmap development and planning</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <ShieldCheck size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Model Risk</h3>
                        <p class="text-sm text-gray-500">Governance frameworks for ML models</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Eye size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Explainable AI</h3>
                        <p class="text-sm text-gray-500">Transparent, interpretable models</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Scale size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Bias Detection</h3>
                        <p class="text-sm text-gray-500">Fairness monitoring and mitigation</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <GitBranch size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">ML Pipelines</h3>
                        <p class="text-sm text-gray-500">Regulatory-compliant infrastructure</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <FileCheck size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">AI Governance</h3>
                        <p class="text-sm text-gray-500">Complete documentation and controls</p>
                    </div>
                </div>
            </div>

        </div>
    </section>

    <Footer />
</main>
