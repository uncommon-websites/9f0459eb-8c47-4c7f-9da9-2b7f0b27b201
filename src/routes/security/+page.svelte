<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import { Lock, Shield, Eye, FileCheck } from 'lucide-svelte';
</script>

<main class="min-h-screen bg-white font-sans text-gray-900 selection:bg-gray-900 selection:text-white">
    <Header />

    <!-- Hero Section - matches homepage SecuritySection -->
    <section class="bg-[#111111] text-white py-24 md:py-32">
        <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-16">
                <!-- Left Content -->
                <div class="flex flex-col justify-center">
                    <div class="flex items-center gap-2 mb-8">
                        <Lock size={16} class="text-white" />
                        <span class="text-xs font-mono uppercase tracking-widest text-gray-400">Security & Compliance</span>
                    </div>

                    <h1 class="text-4xl md:text-5xl lg:text-6xl font-serif leading-[0.95] tracking-[-0.01em] mb-2">Automated</h1>
                    <h1 class="text-4xl md:text-5xl lg:text-6xl font-serif leading-[0.95] tracking-[-0.01em] mb-12">Security Standards</h1>

                    <div class="space-y-4">
                        <div class="flex items-center gap-3">
                            <Lock size={16} class="text-gray-400" />
                            <span class="text-sm font-medium">Financial-grade data protection</span>
                        </div>
                        <div class="flex items-center gap-3">
                            <Shield size={16} class="text-gray-400" />
                            <span class="text-sm font-medium">Regulatory compliance expertise</span>
                        </div>
                        <div class="flex items-center gap-3">
                            <Eye size={16} class="text-gray-400" />
                            <span class="text-sm font-medium">Comprehensive audit trails</span>
                        </div>
                        <div class="flex items-center gap-3">
                            <FileCheck size={16} class="text-gray-400" />
                            <span class="text-sm font-medium">Industry certifications</span>
                        </div>
                    </div>
                </div>

                <!-- Right Content: Certifications Grid -->
                <div class="grid grid-cols-2 border-t border-l border-gray-800">
                    <!-- SOC2 -->
                    <div class="aspect-square border-r border-b border-gray-800 flex flex-col items-center justify-center p-8 relative group">
                        <div class="h-24 w-24 rounded-full border-2 border-gray-600 flex items-center justify-center mb-4 opacity-70 group-hover:opacity-100 transition-opacity">
                            <div class="text-center">
                                <div class="text-[10px] font-bold">AICPA</div>
                                <div class="text-lg font-bold">SOC 2</div>
                            </div>
                        </div>
                        <span class="absolute bottom-4 left-4 text-[10px] text-gray-500 font-mono">SOC2</span>
                    </div>

                    <!-- CCPA -->
                    <div class="aspect-square border-r border-b border-gray-800 flex flex-col items-center justify-center p-8 relative group">
                        <svg viewBox="0 0 24 24" fill="currentColor" class="h-20 w-20 text-gray-400 opacity-70 group-hover:opacity-100 transition-opacity">
                            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 17.93c-3.95-.49-7-3.85-7-7.93 0-.62.08-1.21.21-1.79L9 15v1c0 1.1.9 2 2 2v1.93zm6.9-2.54c-.26-.81-1-1.39-1.9-1.39h-1v-3c0-.55-.45-1-1-1H8v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41c2.93 1.19 5 4.06 5 7.41 0 2.08-.8 3.97-2.1 5.39z"/>
                        </svg>
                        <span class="absolute bottom-4 left-4 text-[10px] text-gray-500 font-mono">CCPA</span>
                    </div>

                    <!-- ISO 27001 -->
                    <div class="aspect-square border-r border-b border-gray-800 flex flex-col items-center justify-center p-8 relative group">
                        <div class="h-24 w-24 rounded-full border-2 border-gray-600 flex items-center justify-center mb-4 opacity-70 group-hover:opacity-100 transition-opacity">
                             <div class="text-center">
                                <div class="text-2xl font-bold">ISO</div>
                            </div>
                        </div>
                        <span class="absolute bottom-4 left-4 text-[10px] text-gray-500 font-mono">ISO 27001</span>
                    </div>

                    <!-- GDPR -->
                    <div class="aspect-square border-r border-b border-gray-800 flex flex-col items-center justify-center p-8 relative group">
                        <div class="relative h-20 w-20 opacity-70 group-hover:opacity-100 transition-opacity">
                            {#each [0, 30, 60, 90, 120, 150, 180, 210, 240, 270, 300, 330] as deg}
                                <div class="absolute top-1/2 left-1/2 h-1 w-1 bg-gray-400 rounded-full" style="transform: translate(-50%, -50%) rotate({deg}deg) translate(30px)"></div>
                            {/each}
                        </div>
                        <span class="absolute bottom-4 left-4 text-[10px] text-gray-500 font-mono">GDPR</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Detailed Security Content -->
    <section class="py-24">
        <div class="mx-auto max-w-4xl px-4 sm:px-6 lg:px-8">
            <div class="space-y-12 text-xl md:text-2xl font-serif text-gray-900 leading-[1.4] tracking-[-0.01em]">
                <p>
                    We work with sensitive financial data every day. Security isn't a feature we add—it's the foundation everything else is built on.
                </p>

                <p class="text-gray-500">
                    Our clients trust us with their most critical systems. We take that responsibility seriously.
                </p>
            </div>

            <!-- Security Pillars -->
            <div class="mt-20 pt-12 border-t border-gray-100">
                <h2 class="text-2xl font-serif text-gray-900 mb-10">Our Security Principles</h2>

                <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                    <div class="bg-gray-50 rounded-2xl p-6">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Lock size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-2">Data Encryption</h3>
                        <p class="text-sm text-gray-500">All data encrypted at rest and in transit using industry-standard AES-256 and TLS 1.3.</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Shield size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-2">Infrastructure Security</h3>
                        <p class="text-sm text-gray-500">Hosted on SOC 2 compliant cloud infrastructure with continuous monitoring and automated threat detection.</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Eye size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-2">Access Controls</h3>
                        <p class="text-sm text-gray-500">Role-based access with multi-factor authentication. Principle of least privilege enforced across all systems.</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <FileCheck size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-2">Compliance</h3>
                        <p class="text-sm text-gray-500">SOC 2 Type II certified. Regular third-party penetration testing and security audits.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <Footer />
</main>
