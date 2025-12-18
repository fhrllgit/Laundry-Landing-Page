<template>
    <div class="min-h-screen bg-gradient-to-br from-blue-50 via-white to-blue-50">
        <div class="px-5 md:px-10 lg:px-20 xl:px-40 py-16 md:py-20">
            <div class="max-w-7xl mx-auto">
                <div class="text-center mb-16 md:mb-20">
                    <div class="inline-block mb-4">
                        <span class="px-4 py-2 bg-blue-100 text-[#2196f3] rounded-full text-sm font-semibold">
                            Layanan Profesional
                        </span>
                    </div>
                    <h1 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-800 mb-4 tracking-tight">
                        Layanan Kami
                    </h1>
                    <p class="text-base md:text-lg text-gray-600 max-w-2xl mx-auto leading-relaxed">
                        Empat layanan utama yang kami sediakan untuk memenuhi kebutuhan laundry Anda dengan kualitas
                        terbaik
                    </p>
                </div>
                <div class="space-y-12 md:space-y-20">
                    <div v-for="(service, index) in services" :key="service.id" :class="[
                        'flex flex-col gap-8 lg:gap-12 items-center group',
                        index % 2 === 0 ? 'lg:flex-row' : 'lg:flex-row-reverse'
                    ]">
                        <div class="w-full lg:w-1/2">
                            <div
                                class="relative overflow-hidden rounded-2xl shadow-xl group-hover:shadow-2xl transition-all duration-500">
                                <div class="aspect-[4/3] overflow-hidden bg-gray-200">
                                    <img :src="service.image" :alt="service.title"
                                        class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" />
                                </div>
                                <div
                                    class="absolute inset-0 bg-gradient-to-t from-blue-900/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-500">
                                </div>
                            </div>
                        </div>
                        <div class="w-full lg:w-1/2 space-y-5">
                            <div
                                class="inline-flex p-3 bg-[#2196f3] text-white rounded-xl shadow-lg group-hover:shadow-xl group-hover:bg-[#087fe1] transition-all duration-300">
                                <component :is="service.icon" class="w-8 h-8" />
                            </div>
                            <h2
                                class="text-2xl md:text-3xl font-bold text-gray-800 group-hover:text-[#087fe1] transition-colors duration-300">
                                {{ service.title }}
                            </h2>
                            <p class="text-gray-600 leading-relaxed text-base md:text-lg">
                                {{ service.description }}
                            </p>
                            <!-- <button class="inline-flex items-center px-6 py-3 bg-[#2196f3] hover:bg-[#087fe1] text-white font-semibold rounded-lg shadow-md hover:shadow-lg transition-all duration-300 transform hover:-translate-y-0.5">
                Pelajari Lebih Lanjut
                <svg class="w-5 h-5 ml-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
                </svg>
              </button> -->
                        </div>
                    </div>
                </div>
                <!-- <div class="mt-20 md:mt-24 text-center">
                    <div class="bg-gradient-to-r from-[#2196f3] to-[#087fe1] rounded-2xl p-8 md:p-12 shadow-2xl">
                        <h3 class="text-2xl md:text-3xl font-bold text-white mb-4">
                            Siap Menggunakan Layanan Kami?
                        </h3>
                        <p class="text-blue-50 mb-6 max-w-2xl mx-auto">
                            Hubungi kami sekarang dan dapatkan diskon 20% untuk pelanggan baru
                        </p>
                        <button
                            class="px-8 py-4 cursor-pointer bg-white text-[#2196f3] font-bold rounded-lg shadow-lg hover:shadow-xl transform hover:-translate-y-1 transition-all duration-300">
                            Hubungi Sekarang
                        </button>
                    </div>
                </div> -->
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue'
import { Sparkles, Droplets, Shirt, Package } from 'lucide-vue-next'

const services = ref([
    {
        id: 1,
        title: "Cuci Kiloan",
        description: "Layanan cuci kiloan dengan harga terjangkau dan kualitas terbaik. Pakaian Anda akan dicuci bersih dengan detergen premium dan pewangi pilihan.",
        icon: Package,
        image: "https://images.unsplash.com/photo-1517677208171-0bc6725a3e60?w=600&q=80"
    },
    {
        id: 2,
        title: "Cuci Setrika",
        description: "Pakaian Anda tidak hanya dicuci bersih, tetapi juga disetrika rapi dan siap pakai. Cocok untuk kebutuhan sehari-hari maupun acara formal.",
        icon: Shirt,
        image: "https://images.unsplash.com/photo-1582735689369-4fe89db7114c?w=600&q=80"
    },
    {
        id: 3,
        title: "Dry Cleaning",
        description: "Perawatan khusus untuk pakaian berbahan sensitif seperti jas, gaun, dan pakaian formal lainnya dengan teknologi dry cleaning modern.",
        icon: Sparkles,
        image: "https://images.unsplash.com/photo-1489274495757-95c7c837b101?w=600&q=80"
    },
    {
        id: 4,
        title: "Express Service",
        description: "Butuh pakaian bersih dalam waktu singkat? Layanan express kami siap membantu dengan waktu pengerjaan hanya 6-12 jam.",
        icon: Droplets,
        image: "https://images.unsplash.com/photo-1567538096630-e0c55bd6374c?w=600&q=80"
    }
])
</script>
