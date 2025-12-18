<script>
    // Icons replaced with CSS shapes for pixel-perfect custom visuals
</script>

<section class="py-24 bg-white">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="mb-16">
            <h2 class="text-4xl md:text-5xl font-serif text-gray-900 leading-[0.95] tracking-[-0.01em]">
                Expert Consultants Meet<br />AI-Augmented Delivery
            </h2>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Deep Expertise -->
            <div class="bg-gray-50 p-8 rounded-lg flex flex-col h-full">
                <h3 class="text-lg font-serif text-gray-900 mb-8">Deep Expertise</h3>
                <div class="flex-1 flex items-center justify-center mb-8">
                    <div class="grid grid-cols-3 gap-4">
                        {#each [1, 2, 3, 4, 5, 6] as i}
                            <div class="h-10 w-10 bg-white rounded-full shadow-sm flex items-center justify-center text-gray-400">
                                <div class="h-4 w-4 bg-primary-200 rounded-sm"></div>
                            </div>
                        {/each}
                    </div>
                </div>
                <p class="text-xs text-gray-500 leading-relaxed mt-auto">
                    Every team member brings 20+ years of specialized experience across financial services, technology, and regulatory compliance domains.
                </p>
            </div>

            <!-- Proven Roadmaps -->
            <div class="bg-gray-50 p-8 rounded-lg flex flex-col h-full">
                <h3 class="text-lg font-serif text-gray-900 mb-8">Proven Roadmaps</h3>
                <div class="flex-1 flex items-center justify-center mb-8">
                    <div class="bg-white p-4 rounded shadow-sm w-full max-w-[200px] space-y-2">
                        <div class="h-2 bg-gray-100 rounded w-1/3 mb-4"></div>
                        {#each [1, 2, 3, 4, 5] as i}
                            <div class="flex items-center gap-2">
                                <div class="h-2 w-2 rounded-full bg-primary-300"></div>
                                <div class="h-1.5 bg-gray-100 rounded w-3/4"></div>
                            </div>
                        {/each}
                    </div>
                </div>
                <p class="text-xs text-gray-500 leading-relaxed mt-auto">
                    Battle-tested modernization roadmaps that overcome legacy system fears and deliver measurable results for financial institutions.
                </p>
            </div>

            <!-- Hands-On Consulting -->
            <div class="bg-gray-50 p-8 rounded-lg flex flex-col h-full">
                <h3 class="text-lg font-serif text-gray-900 mb-8">Hands-On Consulting</h3>
                <div class="flex-1 flex items-center justify-center mb-8">
                    <div class="flex -space-x-2">
                        <div class="h-10 w-10 rounded-full bg-primary-100 border-2 border-white flex items-center justify-center text-primary-700 text-xs">A</div>
                        <div class="h-10 w-10 rounded-full bg-primary-200 border-2 border-white flex items-center justify-center text-primary-800 text-xs">B</div>
                        <div class="h-10 w-10 rounded-full bg-primary-300 border-2 border-white flex items-center justify-center text-primary-900 text-xs">C</div>
                    </div>
                </div>
                <p class="text-xs text-gray-500 leading-relaxed mt-auto">
                    Direct engagement with senior consultants who understand financial services operations, regulatory requirements, and technology transformation.
                </p>
            </div>

            <!-- AI Agents -->
            <div class="bg-gray-50 p-8 rounded-lg flex flex-col h-full">
                <h3 class="text-lg font-serif text-gray-900 mb-8">AI Agents</h3>
                <div class="flex-1 flex items-center justify-center mb-8">
                    <div class="relative">
                        <!-- Tree structure visualization -->
                        <div class="flex justify-center gap-4 mb-4">
                            <div class="h-6 w-6 border border-primary-300 bg-white rounded-sm"></div>
                            <div class="h-6 w-6 border border-primary-300 bg-white rounded-sm"></div>
                            <div class="h-6 w-6 border border-primary-300 bg-white rounded-sm"></div>
                        </div>
                        <div class="flex justify-center mb-4">
                            <div class="h-8 w-px bg-primary-300"></div>
                        </div>
                        <div class="flex justify-center">
                            <div class="h-8 w-8 bg-primary-700 rounded flex items-center justify-center text-white text-xs">AI</div>
                        </div>
                    </div>
                </div>
                <p class="text-xs text-gray-500 leading-relaxed mt-auto">
                    Intelligent automation agents that augment your team's capabilities, handling routine compliance tasks while maintaining accuracy and audit trails.
                </p>
            </div>

            <!-- GRC Compliance -->
            <div class="bg-gray-50 p-8 rounded-lg flex flex-col h-full">
                <h3 class="text-lg font-serif text-gray-900 mb-8">GRC Compliance</h3>
                <div class="flex-1 flex items-center justify-center mb-8">
                    <div class="bg-white p-4 rounded shadow-sm w-full max-w-[200px]">
                        <div class="flex justify-between mb-4">
                            <div class="text-[10px] font-bold">GRC</div>
                            <div class="text-[10px] font-bold text-primary-700">✓</div>
                        </div>
                        <div class="space-y-2">
                            <div class="h-px bg-gray-100 w-full"></div>
                            <div class="h-1.5 bg-primary-100 rounded w-1/2"></div>
                            <div class="h-1.5 bg-primary-100 rounded w-3/4"></div>
                            <div class="h-1.5 bg-primary-100 rounded w-2/3"></div>
                        </div>
                    </div>
                </div>
                <p class="text-xs text-gray-500 leading-relaxed mt-auto">
                    Comprehensive governance, risk, and compliance frameworks designed for financial institutions. Streamline regulatory requirements while maintaining full audit capabilities.
                </p>
            </div>

            <!-- Scalable Solutions -->
            <div class="bg-gray-50 p-8 rounded-lg flex flex-col h-full">
                <h3 class="text-lg font-serif text-gray-900 mb-8">Scalable Solutions</h3>
                <div class="flex-1 flex items-center justify-center mb-8">
                    <div class="grid grid-cols-3 gap-1">
                        {#each [1, 2, 3, 4, 5, 6, 7, 8, 9] as i}
                            <div class={`h-8 w-8 border border-gray-200 ${i === 5 ? 'bg-primary-700 flex items-center justify-center' : 'bg-white'}`}>
                                {#if i === 5}
                                    <div class="h-2 w-2 bg-white rounded-full"></div>
                                {/if}
                            </div>
                        {/each}
                    </div>
                </div>
                <p class="text-xs text-gray-500 leading-relaxed mt-auto">
                    Solutions that scale from initial implementation to enterprise-wide deployment, adapting to your institution's growth and evolving needs.
                </p>
            </div>
        </div>
    </div>
</section>
