<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import { Mail, Phone, MapPin, Calendar } from 'lucide-svelte';

    let formData = {
        name: '',
        email: '',
        company: '',
        message: ''
    };

    let isSubmitting = false;
    let isSubmitted = false;
    let submitError = '';

    async function handleSubmit() {
        isSubmitting = true;
        submitError = '';

        try {
            const response = await fetch('https://api.web3forms.com/submit', {
                method: 'POST',
                headers: {
                    'Content-Type': 'application/json',
                    'Accept': 'application/json'
                },
                body: JSON.stringify({
                    access_key: '493b7183-4619-495d-b8a4-5cf43636c87b',
                    name: formData.name,
                    email: formData.email,
                    company: formData.company,
                    message: formData.message
                })
            });

            const result = await response.json();

            if (result.success) {
                isSubmitted = true;
            } else {
                submitError = result.message || 'Something went wrong. Please try again.';
            }
        } catch (error) {
            submitError = 'Failed to send message. Please try again.';
        } finally {
            isSubmitting = false;
        }
    }
</script>

<main class="min-h-screen bg-white font-sans text-gray-900 selection:bg-gray-900 selection:text-white">
    <Header />

    <section class="py-12 sm:py-16 md:py-24">
        <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-16">
                <!-- Left: Content -->
                <div>
                    <div class="mb-6">
                        <span class="text-[10px] font-mono uppercase tracking-widest text-gray-500">Get in Touch</span>
                    </div>
                    <h1 class="text-4xl md:text-5xl lg:text-6xl font-serif text-gray-900 leading-[0.95] tracking-[-0.01em] mb-8">
                        Let's discuss your<br />modernization goals
                    </h1>
                    <p class="text-lg text-gray-600 leading-relaxed mb-12 max-w-md">
                        Ready to transform your financial operations? Our team of experts is here to help you navigate your GRC modernization journey.
                    </p>

                    <!-- Quick Actions -->
                    <div class="space-y-6 mb-12">
                        <a href="https://calendly.com/jose-altura/30min" target="_blank" rel="noopener noreferrer" class="flex items-center gap-4 p-4 bg-primary-50 rounded-lg hover:bg-primary-100 transition-colors group">
                            <div class="h-12 w-12 rounded-full bg-primary-600 flex items-center justify-center text-white group-hover:bg-primary-700 transition-colors">
                                <Calendar size={20} />
                            </div>
                            <div>
                                <div class="font-medium text-gray-900">Schedule a Consultation</div>
                                <div class="text-sm text-gray-500">Book a 30-minute call with our team</div>
                            </div>
                        </a>

                        <a href="mailto:hello@altura.finance" class="flex items-center gap-4 p-4 bg-gray-50 rounded-lg hover:bg-gray-100 transition-colors">
                            <div class="h-12 w-12 rounded-full bg-gray-200 flex items-center justify-center text-gray-600">
                                <Mail size={20} />
                            </div>
                            <div>
                                <div class="font-medium text-gray-900">Email Us</div>
                                <div class="text-sm text-gray-500">hello@altura.finance</div>
                            </div>
                        </a>
                    </div>

                    <!-- Location -->
                    <div class="flex items-center gap-3 text-sm text-gray-500">
                        <MapPin size={16} />
                        <span>Panamá City, Panamá</span>
                    </div>
                </div>

                <!-- Right: Form -->
                <div class="bg-gray-50 rounded-2xl p-8 lg:p-12">
                    {#if isSubmitted}
                        <div class="h-full flex flex-col items-center justify-center text-center py-12">
                            <div class="h-16 w-16 rounded-full bg-primary-100 flex items-center justify-center text-primary-600 mb-6">
                                <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M20 6 9 17l-5-5"/></svg>
                            </div>
                            <h3 class="text-2xl font-serif text-gray-900 mb-2">Message Sent</h3>
                            <p class="text-gray-500 mb-8">We'll get back to you within 24 hours.</p>
                            <button
                                on:click={() => { isSubmitted = false; formData = { name: '', email: '', company: '', message: '' }; }}
                                class="text-sm font-medium text-primary-600 hover:text-primary-700"
                            >
                                Send another message
                            </button>
                        </div>
                    {:else}
                        <h2 class="text-2xl font-serif text-gray-900 mb-2">Send us a message</h2>
                        <p class="text-sm text-gray-500 mb-8">Fill out the form below and we'll be in touch soon.</p>

                        <form on:submit|preventDefault={handleSubmit} class="space-y-6">
                            <div>
                                <label for="name" class="block text-xs font-medium text-gray-700 mb-2">Full Name</label>
                                <input
                                    type="text"
                                    id="name"
                                    bind:value={formData.name}
                                    required
                                    class="w-full px-4 py-3 bg-white border border-gray-200 rounded-lg text-sm focus:outline-none focus:ring-2 focus:ring-primary-500 focus:border-transparent transition-all"
                                    placeholder="Your full name"
                                />
                            </div>

                            <div>
                                <label for="email" class="block text-xs font-medium text-gray-700 mb-2">Work Email</label>
                                <input
                                    type="email"
                                    id="email"
                                    bind:value={formData.email}
                                    required
                                    class="w-full px-4 py-3 bg-white border border-gray-200 rounded-lg text-sm focus:outline-none focus:ring-2 focus:ring-primary-500 focus:border-transparent transition-all"
                                    placeholder="you@yourcompany.com"
                                />
                            </div>

                            <div>
                                <label for="company" class="block text-xs font-medium text-gray-700 mb-2">Company</label>
                                <input
                                    type="text"
                                    id="company"
                                    bind:value={formData.company}
                                    class="w-full px-4 py-3 bg-white border border-gray-200 rounded-lg text-sm focus:outline-none focus:ring-2 focus:ring-primary-500 focus:border-transparent transition-all"
                                    placeholder="Your company name"
                                />
                            </div>

                            <div>
                                <label for="message" class="block text-xs font-medium text-gray-700 mb-2">How can we help?</label>
                                <textarea
                                    id="message"
                                    bind:value={formData.message}
                                    required
                                    rows="4"
                                    class="w-full px-4 py-3 bg-white border border-gray-200 rounded-lg text-sm focus:outline-none focus:ring-2 focus:ring-primary-500 focus:border-transparent transition-all resize-none"
                                    placeholder="I'm interested in learning more about..."
                                ></textarea>
                            </div>

                            {#if submitError}
                                <div class="p-3 bg-red-50 border border-red-200 rounded-lg text-sm text-red-600">
                                    {submitError}
                                </div>
                            {/if}

                            <button
                                type="submit"
                                disabled={isSubmitting}
                                class="w-full rounded-full bg-black px-8 py-4 text-sm font-medium text-white hover:bg-gray-800 transition-all disabled:opacity-50 disabled:cursor-not-allowed"
                            >
                                {#if isSubmitting}
                                    Sending...
                                {:else}
                                    Send Message
                                {/if}
                            </button>
                        </form>

                        <p class="text-[10px] text-gray-400 mt-6 text-center">
                            By submitting this form, you agree to our privacy policy.
                        </p>
                    {/if}
                </div>
            </div>
        </div>
    </section>

    <Footer />
</main>
