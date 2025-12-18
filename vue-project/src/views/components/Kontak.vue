<template>
    <section class="bg-white px-5 border md:px-10 lg:px-20 xl:px-40 py-16 md:py-20">
        <div class="max-w-7xl border mx-auto">
            <!-- Section Header -->
            <div class="text-center mb-12">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-3">
                    Hubungi Kami
                </h2>
                <p class="text-gray-600 text-lg">
                    Siap melayani laundry Anda kapan saja
                </p>
            </div>

            <!-- Main Layout: 2 Columns -->
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 lg:gap-12">

                <!-- Left Column: Contact Form -->
                <div class="order-2 lg:order-1">
                    <div class="space-y-6">

                        <!-- Nama -->
                        <div>
                            <label for="nama" class="block text-sm font-medium text-gray-700 mb-2">
                                Nama Lengkap
                            </label>
                            <input type="text" id="nama" v-model="formData.nama" placeholder="Masukkan nama Anda"
                                class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:border-blue-500 focus:ring-2 focus:ring-blue-200 outline-none transition-all" />
                        </div>

                        <!-- WhatsApp -->
                        <div>
                            <label for="whatsapp" class="block text-sm font-medium text-gray-700 mb-2">
                                Nomor WhatsApp
                            </label>
                            <input type="tel" id="whatsapp" v-model="formData.whatsapp" placeholder="08xxxxxxxxxx"
                                class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:border-blue-500 focus:ring-2 focus:ring-blue-200 outline-none transition-all" />
                        </div>

                        <!-- Alamat -->
                        <div>
                            <label for="alamat" class="block text-sm font-medium text-gray-700 mb-2">
                                Alamat Lengkap
                            </label>
                            <textarea id="alamat" v-model="formData.alamat" placeholder="Masukkan alamat lengkap Anda"
                                rows="3"
                                class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:border-blue-500 focus:ring-2 focus:ring-blue-200 outline-none transition-all resize-none"></textarea>
                        </div>

                        <!-- Pesan -->
                        <div>
                            <label for="pesan" class="block text-sm font-medium text-gray-700 mb-2">
                                Pesan
                            </label>
                            <textarea id="pesan" v-model="formData.pesan"
                                placeholder="Tuliskan pesan atau pertanyaan Anda" rows="4"
                                class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:border-blue-500 focus:ring-2 focus:ring-blue-200 outline-none transition-all resize-none"></textarea>
                        </div>

                        <!-- Submit Button -->
                        <button @click="handleSubmit"
                            class="w-full bg-blue-500 hover:bg-blue-600 text-white font-semibold py-4 rounded-xl transition-all duration-300 shadow-lg hover:shadow-xl transform hover:-translate-y-0.5">
                            Kirim Pesan
                        </button>
                    </div>
                </div>

                <!-- Right Column: Visual Mockup + Map -->
                <div class="order-1 lg:order-2">
                    <div class="relative">

                        <!-- Smartphone Mockup -->
                        <div class="relative mx-auto max-w-sm">
                            <!-- Phone Frame -->
                            <div class="bg-gray-900 rounded-[3rem] p-3 shadow-2xl">
                                <div class="bg-white rounded-[2.5rem] overflow-hidden">
                                    <!-- Notch -->
                                    <div class="bg-gray-900 h-6 w-32 mx-auto rounded-b-2xl"></div>

                                    <!-- Map Container -->
                                    <div class="aspect-[9/16] relative">
                                        <iframe
                                            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d126748.56211042778!2d110.36437!3d-6.9932484!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e708b4d3f0d024d%3A0x1e0432b9da5cb9f2!2sJepara%2C%20Central%20Java!5e0!3m2!1sen!2sid!4v1234567890"
                                            width="100%" height="100%" style="border:0;" allowfullscreen=""
                                            loading="lazy" referrerpolicy="no-referrer-when-downgrade"
                                            class="absolute inset-0"></iframe>
                                    </div>
                                </div>
                            </div>

                            <!-- Floating Cards -->
                            <!-- Address Card -->
                            <div
                                class="absolute -left-4 top-20 bg-white rounded-2xl shadow-xl p-4 max-w-[200px] animate-float">
                                <div class="flex items-start gap-3">
                                    <div class="bg-blue-100 p-2 rounded-lg flex-shrink-0">
                                        <svg class="w-5 h-5 text-blue-500" fill="none" stroke="currentColor"
                                            viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                                d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                                d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
                                        </svg>
                                    </div>
                                    <div>
                                        <p class="text-xs font-semibold text-gray-900">Lokasi Kami</p>
                                        <p class="text-xs text-gray-600 mt-1">Jl. Contoh No. 123, Jepara</p>
                                    </div>
                                </div>
                            </div>

                            <!-- WhatsApp Card -->
                            <div
                                class="absolute -right-4 bottom-32 bg-white rounded-2xl shadow-xl p-4 max-w-[200px] animate-float-delayed">
                                <div class="flex items-start gap-3">
                                    <div class="bg-green-100 p-2 rounded-lg flex-shrink-0">
                                        <svg class="w-5 h-5 text-green-500" fill="currentColor" viewBox="0 0 24 24">
                                            <path
                                                d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413Z" />
                                        </svg>
                                    </div>
                                    <div>
                                        <p class="text-xs font-semibold text-gray-900">WhatsApp</p>
                                        <p class="text-xs text-gray-600 mt-1">+62 812-3456-7890</p>
                                    </div>
                                </div>
                            </div>

                        </div>

                        <!-- Decorative Background -->
                        <div
                            class="absolute inset-0 bg-gradient-to-br from-blue-50 to-blue-100 rounded-3xl -z-10 transform scale-95 opacity-50">
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue';

const formData = ref({
    nama: '',
    whatsapp: '',
    alamat: '',
    pesan: ''
});

const handleSubmit = () => {
    if (!formData.value.nama || !formData.value.whatsapp || !formData.value.alamat || !formData.value.pesan) {
        alert('Mohon lengkapi semua field!');
        return;
    }

    // Handle form submission
    console.log('Form submitted:', formData.value);
    alert('Terima kasih! Pesan Anda telah terkirim.');

    // Reset form
    formData.value = {
        nama: '',
        whatsapp: '',
        alamat: '',
        pesan: ''
    };
};
</script>

<style scoped>
@keyframes float {

    0%,
    100% {
        transform: translateY(0px);
    }

    50% {
        transform: translateY(-10px);
    }
}

@keyframes float-delayed {

    0%,
    100% {
        transform: translateY(0px);
    }

    50% {
        transform: translateY(-10px);
    }
}

.animate-float {
    animation: float 3s ease-in-out infinite;
}

.animate-float-delayed {
    animation: float-delayed 3s ease-in-out infinite;
    animation-delay: 1.5s;
}

/* Smooth scrolling for mobile */
@media (max-width: 1024px) {
    .order-1 {
        margin-bottom: 2rem;
    }
}
</style>