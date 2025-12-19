<script>
    import { Building2, Shield, TrendingUp, Laptop, Check, Lock, ShieldCheck, KeyRound, Cloud, Server } from 'lucide-svelte';
</script>

<section class="py-24 bg-white">
    <div class="mx-auto max-w-[1400px] px-8 sm:px-12 lg:px-16">
        <div class="mb-16 max-w-2xl">
            <h2 class="text-3xl md:text-4xl font-serif text-gray-900 leading-[0.95] tracking-[-0.01em] mb-6">Trusted by Financial Institutions</h2>
            <p class="text-sm text-gray-500 leading-relaxed">
                We serve regional banks, credit unions, investment firms, insurance and reinsurance companies with enterprise-grade modernization embedded with security and compliance. Our expertise spans the full spectrum of financial services, backed by industry certifications and proven modernization success.
            </p>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4">
            <!-- Industry Partners -->
            <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                <div class="h-8 w-8 rounded flex items-center justify-center bg-gray-200 text-gray-600">
                    <Building2 size={16} />
                </div>
                <span class="text-sm font-medium text-gray-900">Regional Banks</span>
            </div>
            <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                <div class="h-8 w-8 rounded flex items-center justify-center bg-primary-600 text-white">
                    <Shield size={16} />
                </div>
                <span class="text-sm font-medium text-gray-900">Insurance and Reinsurance</span>
            </div>
            <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                <div class="h-8 w-8 rounded flex items-center justify-center bg-primary-700 text-white">
                    <TrendingUp size={16} />
                </div>
                <span class="text-sm font-medium text-gray-900">Investment Firms</span>
            </div>
            <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                <div class="h-8 w-8 rounded flex items-center justify-center bg-primary-800 text-white">
                    <Laptop size={16} />
                </div>
                <span class="text-sm font-medium text-gray-900">Fintech Companies</span>
            </div>

            <!-- Certifications -->
            <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                <div class="h-8 w-8 rounded flex items-center justify-center bg-gray-700 text-white">
                    <Check size={16} />
                </div>
                <span class="text-sm font-medium text-gray-900">SOC 2</span>
            </div>
            <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                <div class="h-8 w-8 rounded flex items-center justify-center bg-gray-800 text-white">
                    <Lock size={16} />
                </div>
                <span class="text-sm font-medium text-gray-900">ISO 27001</span>
            </div>
            <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                <div class="h-8 w-8 rounded flex items-center justify-center bg-gray-200 text-gray-600">
                    <ShieldCheck size={16} />
                </div>
                <span class="text-sm font-medium text-gray-900">GDPR Compliant</span>
            </div>
            <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                <div class="h-8 w-8 rounded flex items-center justify-center bg-gray-200 text-gray-600">
                    <KeyRound size={16} />
                </div>
                <span class="text-sm font-medium text-gray-900">CCPA Compliant</span>
            </div>

            <!-- Cloud Infrastructure -->
            <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                <div class="h-8 w-8 rounded flex items-center justify-center bg-orange-500 text-white">
                    <Cloud size={16} />
                </div>
                <span class="text-sm font-medium text-gray-900">AWS Infrastructure</span>
            </div>
            <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                <div class="h-8 w-8 rounded flex items-center justify-center bg-blue-600 text-white">
                    <Cloud size={16} />
                </div>
                <span class="text-sm font-medium text-gray-900">Azure Integration</span>
            </div>
            <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                <div class="h-8 w-8 rounded flex items-center justify-center bg-blue-500 text-white">
                    <Cloud size={16} />
                </div>
                <span class="text-sm font-medium text-gray-900">GCP</span>
            </div>
            <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                <div class="h-8 w-8 rounded flex items-center justify-center bg-gray-200 text-gray-600">
                    <Server size={16} />
                </div>
                <span class="text-sm font-medium text-gray-900">Enterprise Security</span>
            </div>
        </div>
    </div>
</section>
