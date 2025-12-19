<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import { LayoutDashboard, Settings, Layers, Bell, BarChart3, Link } from 'lucide-svelte';
</script>

<main class="min-h-screen bg-white font-sans text-gray-900 selection:bg-gray-900 selection:text-white">
    <Header />

    <section class="py-12 sm:py-16 md:py-32">
        <div class="mx-auto max-w-4xl px-4 sm:px-6 lg:px-8">
            <div class="mb-12">
                <span class="text-[10px] font-mono uppercase tracking-widest text-gray-500">Services</span>
            </div>

            <h1 class="text-4xl md:text-5xl lg:text-6xl font-serif text-gray-900 leading-[0.95] tracking-[-0.01em] mb-16">
                GRC Modernization
            </h1>

            <div class="space-y-12 text-xl md:text-2xl font-serif text-gray-900 leading-[1.4] tracking-[-0.01em]">
                <p>
                    Legacy GRC systems weren't built for today's regulatory landscape. They create silos, require manual processes, and leave compliance teams drowning in spreadsheets.
                </p>

                <p class="text-gray-500">
                    Modern banking demands a unified approach—one where governance, risk, and compliance work together seamlessly.
                </p>

                <p>
                    <span class="text-primary-700">We transform fragmented GRC operations into integrated platforms</span> that give leadership real-time visibility and reduce the burden on your teams.
                </p>
            </div>

            <!-- What We Deliver -->
            <div class="mt-20 pt-12 border-t border-gray-100">
                <h2 class="text-2xl font-serif text-gray-900 mb-10">What We Deliver</h2>

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <LayoutDashboard size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Unified Dashboards</h3>
                        <p class="text-sm text-gray-500">Risk and compliance visibility in one place</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Settings size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Control Testing</h3>
                        <p class="text-sm text-gray-500">Automated testing and continuous monitoring</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Layers size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Framework Mapping</h3>
                        <p class="text-sm text-gray-500">SOC 2, SOX, NIST cross-mapping</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Bell size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Change Management</h3>
                        <p class="text-sm text-gray-500">Real-time regulatory updates</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <BarChart3 size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Executive Reporting</h3>
                        <p class="text-sm text-gray-500">Board-ready presentations</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Link size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">System Integration</h3>
                        <p class="text-sm text-gray-500">Connect with core banking platforms</p>
                    </div>
                </div>
            </div>

        </div>
    </section>

    <Footer />
</main>
