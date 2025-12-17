<script>
    const partners = [
        { name: "Regional Banks", icon: "🏦" },
        { name: "Credit Unions", icon: "💳", color: "bg-primary-600" },
        { name: "Investment Firms", icon: "📈", color: "bg-primary-700" },
        { name: "Fintech Companies", icon: "💻", color: "bg-primary-800" },
        { name: "SOC 2 Certified", icon: "✓", color: "bg-gray-700" },
        { name: "ISO 27001", icon: "🔒", color: "bg-gray-800" },
        { name: "GDPR Compliant", icon: "🛡️" },
        { name: "CCPA Compliant", icon: "🔐" },
        { name: "AWS Infrastructure", icon: "☁️", color: "bg-orange-500" },
        { name: "Azure Integration", icon: "☁️", color: "bg-blue-600" },
        { name: "GCP Compatible", icon: "☁️", color: "bg-blue-500" },
        { name: "Enterprise Security", icon: "🔑" }
    ];
</script>

<section class="py-24 bg-white">
    <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="mb-16 max-w-2xl">
            <h2 class="text-3xl md:text-4xl font-serif text-gray-900 mb-6">Trusted by Financial Institutions</h2>
            <p class="text-sm text-gray-500 leading-relaxed">
                We serve regional banks, credit unions, and investment firms with enterprise-grade security and compliance. Our expertise spans the full spectrum of financial services, backed by industry certifications and proven modernization success.
            </p>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4">
            {#each partners as partner}
                <div class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors cursor-default">
                    <div class={`h-8 w-8 rounded flex items-center justify-center text-white text-xs font-bold ${partner.color ? partner.color : 'bg-gray-200 text-gray-600'}`}>
                        {partner.icon}
                    </div>
                    <span class="text-sm font-medium text-gray-900">{partner.name}</span>
                </div>
            {/each}
        </div>
    </div>
</section>
