<script>
    import { Target, Users, Clock, Award } from 'lucide-svelte';
</script>

<section class="bg-[#F9F7F2] py-12 sm:py-16 md:py-24 overflow-hidden">
    <div class="mx-auto max-w-[1400px] px-5 sm:px-12 lg:px-16">
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-10 sm:gap-12 lg:gap-16 items-center">
            <!-- Left: Founder Quote -->
            <div>
                <div class="mb-4 sm:mb-6">
                    <span class="text-[10px] font-mono uppercase tracking-widest text-gray-500">Our Mission</span>
                </div>
                <blockquote class="text-xl sm:text-2xl md:text-3xl font-serif text-gray-900 leading-[1.3] tracking-[-0.01em] mb-6 sm:mb-8 md:mb-10">
                    "Financial institutions deserve modernization partners who understand both the technology and the regulatory landscape. We built Altura to bridge that gap—combining deep GRC expertise with AI-powered delivery."
                </blockquote>
                <div class="flex items-center gap-4">
                    <div class="h-12 w-12 rounded-full bg-gray-900 flex items-center justify-center text-white font-medium">
                        JG
                    </div>
                    <div>
                        <div class="font-medium text-gray-900">José Abraham García</div>
                        <div class="text-[10px] uppercase tracking-widest text-gray-500 mt-0.5">Founder & Managing Director</div>
                    </div>
                </div>
            </div>

            <!-- Right: Stats Grid -->
            <div class="grid grid-cols-2 gap-3 sm:gap-4 md:gap-6">
                <div class="bg-white p-4 sm:p-5 md:p-6 rounded-lg">
                    <div class="flex items-center gap-3 mb-3 sm:mb-4">
                        <div class="h-8 w-8 sm:h-10 sm:w-10 rounded-full bg-primary-100 flex items-center justify-center text-primary-700">
                            <Clock class="h-4 w-4 sm:h-5 sm:w-5" />
                        </div>
                    </div>
                    <div class="text-2xl sm:text-3xl font-serif text-gray-900 mb-1">20+</div>
                    <div class="text-[10px] sm:text-xs text-gray-500">Years of combined experience in financial services</div>
                </div>

                <div class="bg-white p-4 sm:p-5 md:p-6 rounded-lg">
                    <div class="flex items-center gap-3 mb-3 sm:mb-4">
                        <div class="h-8 w-8 sm:h-10 sm:w-10 rounded-full bg-primary-100 flex items-center justify-center text-primary-700">
                            <Target class="h-4 w-4 sm:h-5 sm:w-5" />
                        </div>
                    </div>
                    <div class="text-2xl sm:text-3xl font-serif text-gray-900 mb-1">100%</div>
                    <div class="text-[10px] sm:text-xs text-gray-500">Focus on regulated industries</div>
                </div>

                <div class="bg-white p-4 sm:p-5 md:p-6 rounded-lg">
                    <div class="flex items-center gap-3 mb-3 sm:mb-4">
                        <div class="h-8 w-8 sm:h-10 sm:w-10 rounded-full bg-primary-100 flex items-center justify-center text-primary-700">
                            <Users class="h-4 w-4 sm:h-5 sm:w-5" />
                        </div>
                    </div>
                    <div class="text-2xl sm:text-3xl font-serif text-gray-900 mb-1">Hands-on</div>
                    <div class="text-[10px] sm:text-xs text-gray-500">Senior consultants on every engagement</div>
                </div>

                <div class="bg-white p-4 sm:p-5 md:p-6 rounded-lg">
                    <div class="flex items-center gap-3 mb-3 sm:mb-4">
                        <div class="h-8 w-8 sm:h-10 sm:w-10 rounded-full bg-primary-100 flex items-center justify-center text-primary-700">
                            <Award class="h-4 w-4 sm:h-5 sm:w-5" />
                        </div>
                    </div>
                    <div class="text-2xl sm:text-3xl font-serif text-gray-900 mb-1">AI-First</div>
                    <div class="text-[10px] sm:text-xs text-gray-500">Augmented delivery for faster results</div>
                </div>
            </div>
        </div>
    </div>
</section>
