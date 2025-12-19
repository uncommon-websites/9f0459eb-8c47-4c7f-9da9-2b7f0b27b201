<script>
    import { Check, ArrowRight, Shield, Database, Bot } from 'lucide-svelte';
</script>

<section id="services" class="py-12 sm:py-16 md:py-24 bg-white">
    <div class="mx-auto max-w-[1400px] px-5 sm:px-12 lg:px-16">
        <div class="mb-8 sm:mb-12 md:mb-16">
            <h2 class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl font-serif text-gray-900 leading-[1.1] sm:leading-[0.95] tracking-[-0.01em]">
                From Strategy to Execution<br />Here's How We Deliver
            </h2>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 sm:gap-8">
            <!-- Card 1: Compliance Automation -->
            <div>
                <div class="mb-6 bg-[#0B231E] rounded-lg p-6 aspect-[4/3] relative overflow-hidden flex items-center justify-center">
                    <!-- Mock Interface: Compliance Dashboard -->
                    <div class="bg-white rounded-lg p-5 shadow-lg w-full max-w-[92%]">
                        <div class="flex items-center justify-between mb-3 border-b pb-2">
                            <div class="flex items-center gap-2">
                                <Shield size={12} class="text-primary-600" />
                                <span class="text-[10px] font-medium text-gray-700">Compliance Tasks</span>
                            </div>
                            <span class="text-[9px] text-primary-600 font-medium">4/6 Complete</span>
                        </div>
                        <div class="space-y-2">
                            <div class="flex items-center gap-2 text-xs">
                                <div class="h-3.5 w-3.5 rounded border-2 border-primary-500 bg-primary-500 flex items-center justify-center">
                                    <Check size={10} class="text-white" />
                                </div>
                                <span class="text-gray-500 line-through">SOC 2 audit preparation</span>
                            </div>
                            <div class="flex items-center gap-2 text-xs">
                                <div class="h-3.5 w-3.5 rounded border-2 border-primary-500 bg-primary-500 flex items-center justify-center">
                                    <Check size={10} class="text-white" />
                                </div>
                                <span class="text-gray-500 line-through">Risk assessment review</span>
                            </div>
                            <div class="flex items-center gap-2 text-xs">
                                <div class="h-3.5 w-3.5 rounded border-2 border-gray-300 bg-white"></div>
                                <span class="text-gray-700">Vendor compliance check</span>
                            </div>
                            <div class="flex items-center gap-2 text-xs">
                                <div class="h-3.5 w-3.5 rounded border-2 border-gray-300 bg-white"></div>
                                <span class="text-gray-700">Policy documentation</span>
                            </div>
                        </div>
                    </div>
                </div>
                <h3 class="text-xl font-serif text-gray-900 mb-3">Compliance Automation</h3>
                <p class="text-sm text-gray-500 leading-relaxed">
                    Streamline regulatory compliance with AI-powered automation that reduces manual effort and ensures accuracy. Our expert consultants design workflows tailored to your institution's specific GRC requirements.
                </p>
            </div>

            <!-- Card 2: Legacy System Modernization -->
            <div>
                <div class="mb-6 bg-[#0B231E] rounded-lg p-6 aspect-[4/3] relative overflow-hidden flex items-center justify-center">
                     <!-- Mock Interface: System Migration -->
                     <div class="bg-white rounded-lg p-5 shadow-lg w-full max-w-[92%]">
                        <div class="flex items-center gap-2 mb-3">
                            <Database size={12} class="text-primary-600" />
                            <span class="text-[10px] font-medium text-gray-700">System Migration</span>
                        </div>
                        <div class="space-y-3">
                            <div>
                                <div class="flex justify-between text-[9px] mb-1">
                                    <span class="text-gray-500">Legacy → Modern</span>
                                    <span class="text-primary-600 font-medium">78%</span>
                                </div>
                                <div class="h-1.5 bg-gray-100 rounded-full overflow-hidden">
                                    <div class="h-full bg-primary-500 rounded-full animate-progress-fill"></div>
                                </div>
                            </div>
                            <div class="grid grid-cols-2 gap-2 pt-2 border-t">
                                <div class="text-center p-2 bg-gray-50 rounded">
                                    <div class="text-[10px] font-bold text-gray-900">2.4M</div>
                                    <div class="text-[8px] text-gray-400">Records migrated</div>
                                </div>
                                <div class="text-center p-2 bg-gray-50 rounded">
                                    <div class="text-[10px] font-bold text-primary-600">99.9%</div>
                                    <div class="text-[8px] text-gray-400">Data integrity</div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <h3 class="text-xl font-serif text-gray-900 mb-3">Legacy System Modernization</h3>
                <p class="text-sm text-gray-500 leading-relaxed">
                    Transform outdated systems with proven modernization roadmaps. Our 20+ years of experience ensures seamless integration of new technologies while maintaining operational continuity and data integrity.
                </p>
            </div>

            <!-- Card 3: AI Implementation -->
            <div>
                <div class="mb-6 bg-[#0B231E] rounded-lg p-6 aspect-[4/3] relative overflow-hidden flex items-center justify-center">
                     <!-- Mock Interface: AI Agent -->
                     <div class="bg-white rounded-lg p-5 shadow-lg w-full max-w-[92%]">
                        <div class="flex items-center gap-2 mb-3">
                            <div class="h-5 w-5 bg-gradient-to-br from-primary-500 to-primary-700 rounded flex items-center justify-center">
                                <Bot size={12} class="text-white" />
                            </div>
                            <span class="text-[10px] font-medium text-gray-700">AI Agent Active</span>
                            <span class="ml-auto h-1.5 w-1.5 rounded-full bg-green-500 animate-pulse-slow"></span>
                        </div>
                        <div class="space-y-2 text-[9px]">
                            <div class="bg-gray-50 rounded p-2 text-gray-600">
                                Analyzing Q4 compliance reports across 12 departments<span class="animate-typing-dots">...</span>
                            </div>
                            <div class="flex items-center gap-2 text-gray-500">
                                <div class="flex -space-x-1">
                                    <div class="h-4 w-4 rounded-full bg-primary-100 border border-white"></div>
                                    <div class="h-4 w-4 rounded-full bg-primary-200 border border-white"></div>
                                    <div class="h-4 w-4 rounded-full bg-primary-300 border border-white"></div>
                                </div>
                                <span>3 tasks automated today</span>
                            </div>
                        </div>
                    </div>
                </div>
                <h3 class="text-xl font-serif text-gray-900 mb-3">AI Implementation</h3>
                <p class="text-sm text-gray-500 leading-relaxed">
                    Deploy AI agents that augment your team's capabilities while maintaining compliance standards. Our consultants guide implementation from strategy through execution, ensuring measurable results.
                </p>
            </div>
        </div>
    </div>
</section>

<style>
    @keyframes progress-fill {
        0% { width: 0%; }
        100% { width: 78%; }
    }
    .animate-progress-fill {
        animation: progress-fill 2s ease-out forwards;
    }

    @keyframes pulse-slow {
        0%, 100% { opacity: 1; }
        50% { opacity: 0.4; }
    }
    .animate-pulse-slow {
        animation: pulse-slow 2s ease-in-out infinite;
    }

    @keyframes typing-dots {
        0%, 20% { content: '.'; }
        40% { content: '..'; }
        60%, 100% { content: '...'; }
    }
    .animate-typing-dots {
        animation: blink 1.5s steps(1) infinite;
    }
    @keyframes blink {
        0%, 100% { opacity: 1; }
        50% { opacity: 0.3; }
    }
</style>
