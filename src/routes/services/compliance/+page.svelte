<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import { FolderSearch, Activity, FileText, History, Calendar, Users } from 'lucide-svelte';
</script>

<main class="min-h-screen bg-white font-sans text-gray-900 selection:bg-gray-900 selection:text-white">
    <Header />

    <section class="py-12 sm:py-16 md:py-32">
        <div class="mx-auto max-w-4xl px-4 sm:px-6 lg:px-8">
            <div class="mb-12">
                <span class="text-[10px] font-mono uppercase tracking-widest text-gray-500">Services</span>
            </div>

            <h1 class="text-4xl md:text-5xl lg:text-6xl font-serif text-gray-900 leading-[0.95] tracking-[-0.01em] mb-16">
                Compliance Automation
            </h1>

            <div class="space-y-12 text-xl md:text-2xl font-serif text-gray-900 leading-[1.4] tracking-[-0.01em]">
                <p>
                    Manual compliance workflows consume thousands of hours annually. Evidence collection, control testing, audit preparation—all repetitive tasks that pull your best people away from strategic work.
                </p>

                <p class="text-gray-500">
                    Every hour spent on manual data entry is an hour not spent strengthening your security posture.
                </p>

                <p>
                    <span class="text-primary-700">Our AI-powered automation handles the tedious work</span> so your compliance team can focus on risk analysis and strategic decision-making.
                </p>
            </div>

            <!-- What We Deliver -->
            <div class="mt-20 pt-12 border-t border-gray-100">
                <h2 class="text-2xl font-serif text-gray-900 mb-10">What We Deliver</h2>

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <FolderSearch size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Evidence Collection</h3>
                        <p class="text-sm text-gray-500">Automated pipelines for audit evidence</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Activity size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Control Monitoring</h3>
                        <p class="text-sm text-gray-500">Continuous, real-time oversight</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <FileText size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Policy Documentation</h3>
                        <p class="text-sm text-gray-500">AI-assisted policy creation</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <History size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Audit Trails</h3>
                        <p class="text-sm text-gray-500">Complete activity logging</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Calendar size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Deadline Tracking</h3>
                        <p class="text-sm text-gray-500">Never miss regulatory deadlines</p>
                    </div>

                    <div class="bg-gray-50 rounded-2xl p-6 hover:bg-gray-100 transition-colors">
                        <div class="h-10 w-10 rounded-xl bg-primary-100 flex items-center justify-center text-primary-600 mb-4">
                            <Users size={20} />
                        </div>
                        <h3 class="font-medium text-gray-900 mb-1">Vendor Assessments</h3>
                        <p class="text-sm text-gray-500">Automated third-party risk reviews</p>
                    </div>
                </div>
            </div>

        </div>
    </section>

    <Footer />
</main>
