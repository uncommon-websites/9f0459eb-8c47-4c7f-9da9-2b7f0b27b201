<script>
    import { FileText, Database, Settings, Search } from 'lucide-svelte';
</script>

<section id="solutions" class="py-12 sm:py-16 md:py-24 bg-white">
    <div class="mx-auto max-w-[1400px] px-5 sm:px-12 lg:px-16">
        <div class="mb-10 sm:mb-16 md:mb-20">
            <h2 class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl font-serif text-gray-900 leading-[1.1] sm:leading-[0.95] tracking-[-0.01em] max-w-4xl">
                The <span class="font-semibold">modernization partner with AI expertise</span> built for regulated industries
            </h2>
        </div>

        <div class="flex flex-col lg:flex-row lg:items-center lg:justify-between gap-8 sm:gap-10 lg:gap-16">
            <!-- Left: Interface with Grid Background -->
            <div class="relative lg:w-[52%] lg:flex-shrink-0">
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
            <div class="lg:w-[42%]">
                <h3 class="text-2xl font-serif text-gray-900 mb-10">
                    Expert Consultants + AI Agents <br/> Delivering Proven Results
                </h3>

                <div class="grid grid-cols-2 gap-4">
                    {#each [
                        { id: '01', title: 'GRC modernization expertise', icon: Database, desc: 'Deep regulatory knowledge' },
                        { id: '02', title: 'Legacy system transformation', icon: Search, desc: 'Seamless migration paths' },
                        { id: '03', title: 'AI-augmented implementation', icon: Settings, desc: 'Intelligent automation' },
                        { id: '04', title: 'Proven modernization roadmaps', icon: FileText, desc: 'Battle-tested strategies' }
                    ] as feature, i}
                        <div
                            class="group relative p-5 rounded-lg border border-gray-100 bg-white hover:border-gray-200 hover:bg-gray-50/50 hover:-translate-y-0.5 transition-all duration-200 cursor-pointer"
                        >
                            <!-- Left accent bar -->
                            <div class="absolute left-0 top-3 bottom-3 w-0.5 bg-primary-600 rounded-full scale-y-0 group-hover:scale-y-100 transition-transform duration-200 origin-top"></div>

                            <div class="flex items-center justify-between mb-3">
                                <div class="h-9 w-9 rounded-lg bg-primary-900 flex items-center justify-center text-white">
                                    <svelte:component this={feature.icon} size={16} strokeWidth={1.5} />
                                </div>
                                <span class="text-[10px] font-mono text-gray-300 group-hover:text-primary-600 transition-colors">{feature.id}</span>
                            </div>

                            <h4 class="text-sm font-medium text-gray-900 leading-snug mb-1.5">
                                {feature.title}
                            </h4>

                            <p class="text-xs text-gray-400">
                                {feature.desc}
                            </p>
                        </div>
                    {/each}
                </div>
            </div>
        </div>
    </div>
</section>
