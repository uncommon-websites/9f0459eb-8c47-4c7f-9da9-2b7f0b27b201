<script>
    import { Target, Users, Clock, Award } from 'lucide-svelte';
</script>

<section class="bg-[#F9F7F2] py-24 overflow-hidden">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
            <!-- Left: Founder Quote -->
            <div>
                <div class="mb-6">
                    <span class="text-[10px] font-mono uppercase tracking-widest text-gray-500">Our Mission</span>
                </div>
                <blockquote class="text-2xl md:text-3xl font-serif text-gray-900 leading-[1.3] tracking-[-0.01em] mb-10">
                    "Financial institutions deserve modernization partners who understand both the technology and the regulatory landscape. We built Altura to bridge that gap—combining deep GRC expertise with AI-powered delivery."
                </blockquote>
                <div class="flex items-center gap-4">
                    <div class="h-12 w-12 rounded-full bg-gray-900 flex items-center justify-center text-white font-medium">
                        JA
                    </div>
                    <div>
                        <div class="font-medium text-gray-900">Jose Altura</div>
                        <div class="text-[10px] uppercase tracking-widest text-gray-500 mt-0.5">Founder & CEO</div>
                    </div>
                </div>
            </div>

            <!-- Right: Stats Grid -->
            <div class="grid grid-cols-2 gap-6">
                <div class="bg-white p-6 rounded-lg">
                    <div class="flex items-center gap-3 mb-4">
                        <div class="h-10 w-10 rounded-full bg-primary-100 flex items-center justify-center text-primary-700">
                            <Clock size={20} />
                        </div>
                    </div>
                    <div class="text-3xl font-serif text-gray-900 mb-1">20+</div>
                    <div class="text-xs text-gray-500">Years of combined experience in financial services</div>
                </div>

                <div class="bg-white p-6 rounded-lg">
                    <div class="flex items-center gap-3 mb-4">
                        <div class="h-10 w-10 rounded-full bg-primary-100 flex items-center justify-center text-primary-700">
                            <Target size={20} />
                        </div>
                    </div>
                    <div class="text-3xl font-serif text-gray-900 mb-1">100%</div>
                    <div class="text-xs text-gray-500">Focus on regulated industries</div>
                </div>

                <div class="bg-white p-6 rounded-lg">
                    <div class="flex items-center gap-3 mb-4">
                        <div class="h-10 w-10 rounded-full bg-primary-100 flex items-center justify-center text-primary-700">
                            <Users size={20} />
                        </div>
                    </div>
                    <div class="text-3xl font-serif text-gray-900 mb-1">Hands-on</div>
                    <div class="text-xs text-gray-500">Senior consultants on every engagement</div>
                </div>

                <div class="bg-white p-6 rounded-lg">
                    <div class="flex items-center gap-3 mb-4">
                        <div class="h-10 w-10 rounded-full bg-primary-100 flex items-center justify-center text-primary-700">
                            <Award size={20} />
                        </div>
                    </div>
                    <div class="text-3xl font-serif text-gray-900 mb-1">AI-First</div>
                    <div class="text-xs text-gray-500">Augmented delivery for faster results</div>
                </div>
            </div>
        </div>
    </div>
</section>
