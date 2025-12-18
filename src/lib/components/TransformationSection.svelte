<script>
    import { FileText, Database, Settings, Search } from 'lucide-svelte';
</script>

<section id="solutions" class="py-24 bg-white">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="mb-20">
            <h2 class="text-4xl md:text-5xl font-serif text-gray-900 leading-[0.95] tracking-[-0.01em] max-w-4xl">
                The <span class="font-semibold">modernization partner with AI expertise</span> built for regulated industries
            </h2>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
            <!-- Left: Interface with Grid Background -->
            <div class="relative">
                <div class="relative rounded-lg overflow-hidden aspect-[4/3] bg-primary-900">
                    <!-- Grid Pattern -->
                    <div class="absolute inset-0 opacity-20" style="background-image: linear-gradient(to right, rgba(255,255,255,0.1) 1px, transparent 1px), linear-gradient(to bottom, rgba(255,255,255,0.1) 1px, transparent 1px); background-size: 40px 40px;"></div>

                    <!-- Floating Interface Element -->
                    <div class="absolute inset-0 flex items-center justify-center p-8">
                        <div class="bg-white rounded-lg shadow-xl w-full max-w-md p-6">
                            <div class="flex items-center gap-3 mb-4">
                                <div class="h-8 w-8 bg-primary-600 rounded flex items-center justify-center text-white">
                                    <Settings size={16} />
                                </div>
                                <span class="font-medium text-gray-900">GRC Compliance</span>
                            </div>
                            <div class="space-y-2">
                                <div class="h-2 bg-gray-100 rounded w-3/4"></div>
                                <div class="h-2 bg-gray-100 rounded w-1/2"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Right: Features List -->
            <div class="space-y-12">
                <h3 class="text-2xl font-serif text-gray-900">
                    Expert Consultants + AI Agents <br/> Delivering Proven Results
                </h3>

                <div class="space-y-8">
                    {#each [
                        { id: '01', title: 'GRC modernization expertise', icon: Database },
                        { id: '02', title: 'Legacy system transformation', icon: Search },
                        { id: '03', title: 'AI-augmented implementation', icon: Settings },
                        { id: '04', title: 'Proven modernization roadmaps', icon: FileText }
                    ] as feature}
                        <div class="flex items-start gap-4 group cursor-pointer">
                            <div class="flex-shrink-0 relative">
                                <div class="h-10 w-10 rounded-full border border-gray-200 flex items-center justify-center text-xs font-mono text-gray-500 group-hover:border-black group-hover:text-black transition-colors bg-white z-10 relative">
                                    {feature.id}
                                </div>
                                {#if feature.id !== '04'}
                                    <div class="absolute top-10 left-1/2 -translate-x-1/2 w-px h-8 bg-gray-100 -z-0"></div>
                                {/if}
                            </div>
                            <div class="pt-2">
                                <h4 class="text-lg text-gray-600 group-hover:text-gray-900 transition-colors font-light">
                                    {feature.title}
                                </h4>
                            </div>
                        </div>
                    {/each}
                </div>
            </div>
        </div>
    </div>
</section>
