<template>
    <section class="relative border w-full flex py-12 sm:py-16 md:py-20 lg:py-24 bg-white overflow-hidden">
        <div class="pointer-events-none absolute top-0 left-0 w-full h-16 sm:h-20 md:h-24 bg-gradient-to-b from-white via-white/80 to-transparent z-20">
        </div>
        <div class="pointer-events-none absolute bottom-0 left-0 w-full h-16 sm:h-20 md:h-24 bg-gradient-to-t from-white via-white/80 to-transparent z-20">
        </div>

        <div class="absolute inset-0 overflow-hidden opacity-30 sm:opacity-40">
            <div
                class="absolute top-10 sm:top-20 right-8 sm:right-16 lg:right-32 w-40 sm:w-56 md:w-72 h-40 sm:h-56 md:h-72 bg-gradient-to-br from-blue-400/20 to-cyan-300/10 rounded-full blur-3xl animate-pulse">
            </div>
            <div class="absolute bottom-20 sm:bottom-32 md:bottom-40 left-8 sm:left-12 lg:left-20 w-56 sm:w-72 md:w-96 h-56 sm:h-72 md:h-96 bg-gradient-to-tr from-cyan-300/15 to-transparent rounded-full blur-3xl animate-pulse"
                style="animation-delay: 1s;"></div>
            <div
                class="absolute top-20 sm:top-32 md:top-40 right-10 sm:right-16 lg:right-20 w-12 sm:w-16 md:w-20 h-12 sm:h-16 md:h-20 border-2 border-blue-400/20 rounded-2xl rotate-45 animate-float">
            </div>
            <div class="absolute bottom-1/3 left-1/4 w-10 sm:w-12 md:w-16 h-10 sm:h-12 md:h-16 border-2 border-cyan-300/20 rounded-xl rotate-12 animate-float"
                style="animation-delay: 0.5s;"></div>
            <div class="absolute top-1/2 right-1/3 w-12 sm:w-16 md:w-20 h-12 sm:w-16 md:h-20 border-2 border-blue-300/15 rounded-lg rotate-90 animate-float"
                style="animation-delay: 1.5s;"></div>
        </div>

        <div class="container border w-full  relative z-10">
            <div class="text-center mb-10 sm:mb-12 md:mb-16">
                <div class="inline-block mb-4">
                    <div
                        class="flex items-center gap-2 bg-gradient-to-r from-blue-500 to-cyan-400 text-white px-4 py-2 rounded-full text-sm font-semibold">
                        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z">
                            </path>
                        </svg>
                        Hubungi Kami
                    </div>
                </div>
                <h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-gray-900 mb-3 sm:mb-4">
                    Laundry Express 24/7
                </h2>
                <p class="text-gray-600 text-base sm:text-lg mt-4 sm:mt-6 max-w-2xl mx-auto leading-relaxed px-4">
                    Layanan laundry profesional siap melayani kebutuhan Anda kapan saja, di mana saja
                </p>
            </div>

            <div class="border flex gap-8 sm:gap-10 lg:gap-16">
                <div class="space-y-4 sm:space-y-6">
                    <div
                        class="group bg-white/90 backdrop-blur-sm rounded-2xl sm:rounded-3xl p-6 sm:p-8 shadow-lg hover:shadow-2xl transition-all duration-300 border border-gray-100 hover:border-blue-400/30">
                        <div class="flex items-start gap-4 sm:gap-5">
                            <div
                                class="flex-shrink-0 w-12 h-12 sm:w-14 sm:h-14 rounded-xl sm:rounded-2xl bg-gradient-to-br from-blue-500 to-cyan-400 flex items-center justify-center shadow-lg shadow-blue-500/25 group-hover:scale-110 transition-transform">
                                <svg class="w-6 h-6 sm:w-7 sm:h-7 text-white" fill="none" stroke="currentColor"
                                    viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z">
                                    </path>
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path>
                                </svg>
                            </div>
                            <div class="flex-1">
                                <h3 class="text-lg sm:text-xl font-bold text-gray-900 mb-2">Alamat Kami</h3>
                                <p class="text-gray-600 leading-relaxed text-sm sm:text-base">
                                    Jl. Jepara Kedung No. 12, Kecamatan Bae<br>
                                    Kota Jepara, Jawa Tengah, Indonesia
                                </p>
                            </div>
                        </div>
                    </div>

                    <!-- Contact Grid -->
                    <div class="grid sm:grid-cols-2 gap-4 sm:gap-6">
                        <!-- Phone Card -->
                        <div
                            class="group bg-white/90 backdrop-blur-sm rounded-2xl sm:rounded-3xl p-5 sm:p-6 shadow-lg hover:shadow-2xl transition-all duration-300 border border-gray-100 hover:border-blue-400/30">
                            <div
                                class="w-10 h-10 sm:w-12 sm:h-12 rounded-xl bg-gradient-to-br from-blue-500 to-cyan-400 flex items-center justify-center mb-3 sm:mb-4 group-hover:scale-110 transition-transform shadow-lg shadow-blue-500/20">
                                <svg class="w-5 h-5 sm:w-6 sm:h-6 text-white" fill="none" stroke="currentColor"
                                    viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z">
                                    </path>
                                </svg>
                            </div>
                            <h3 class="text-base sm:text-lg font-bold text-gray-900 mb-1 sm:mb-2">Telepon</h3>
                            <p class="text-blue-500 font-semibold text-sm sm:text-base">(021) 1234-5678</p>
                        </div>

                        <!-- WhatsApp Card -->
                        <div
                            class="group bg-white/90 backdrop-blur-sm rounded-2xl sm:rounded-3xl p-5 sm:p-6 shadow-lg hover:shadow-2xl transition-all duration-300 border border-gray-100 hover:border-green-400/30">
                            <div
                                class="w-10 h-10 sm:w-12 sm:h-12 rounded-xl bg-gradient-to-br from-green-500 to-green-400 flex items-center justify-center mb-3 sm:mb-4 group-hover:scale-110 transition-transform shadow-lg shadow-green-500/20">
                                <svg class="w-5 h-5 sm:w-6 sm:h-6 text-white" fill="currentColor" viewBox="0 0 24 24">
                                    <path
                                        d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413Z" />
                                </svg>
                            </div>
                            <h3 class="text-base sm:text-lg font-bold text-gray-900 mb-1 sm:mb-2">WhatsApp</h3>
                            <p class="text-green-600 font-semibold text-sm sm:text-base">0812-3456-7890</p>
                        </div>

                        <!-- Email Card -->
                        <div
                            class="group bg-white/90 backdrop-blur-sm rounded-2xl sm:rounded-3xl p-5 sm:p-6 shadow-lg hover:shadow-2xl transition-all duration-300 border border-gray-100 hover:border-cyan-400/30">
                            <div
                                class="w-10 h-10 sm:w-12 sm:h-12 rounded-xl bg-gradient-to-br from-cyan-500 to-blue-400 flex items-center justify-center mb-3 sm:mb-4 group-hover:scale-110 transition-transform shadow-lg shadow-cyan-500/20">
                                <svg class="w-5 h-5 sm:w-6 sm:h-6 text-white" fill="none" stroke="currentColor"
                                    viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z">
                                    </path>
                                </svg>
                            </div>
                            <h3 class="text-base sm:text-lg font-bold text-gray-900 mb-1 sm:mb-2">Email</h3>
                            <p class="text-cyan-600 font-semibold text-xs sm:text-sm break-all">info@laundryexpress.com
                            </p>
                        </div>

                        <!-- Instagram Card -->
                        <div
                            class="group bg-white/90 backdrop-blur-sm rounded-2xl sm:rounded-3xl p-5 sm:p-6 shadow-lg hover:shadow-2xl transition-all duration-300 border border-gray-100 hover:border-pink-400/30">
                            <div
                                class="w-10 h-10 sm:w-12 sm:h-12 rounded-xl bg-gradient-to-br from-pink-500 via-purple-500 to-orange-400 flex items-center justify-center mb-3 sm:mb-4 group-hover:scale-110 transition-transform shadow-lg shadow-pink-500/20">
                                <svg class="w-5 h-5 sm:w-6 sm:h-6 text-white" fill="currentColor" viewBox="0 0 24 24">
                                    <path
                                        d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z" />
                                </svg>
                            </div>
                            <h3 class="text-base sm:text-lg font-bold text-gray-900 mb-1 sm:mb-2">Instagram</h3>
                            <p class="text-pink-600 font-semibold text-sm sm:text-base">@laundryexpress</p>
                        </div>
                    </div>

                    <!-- Operating Hours Card -->
                    <div
                        class="group bg-gradient-to-br from-blue-50/50 via-white to-cyan-50/30 backdrop-blur-sm rounded-2xl sm:rounded-3xl p-6 sm:p-8 shadow-lg hover:shadow-2xl transition-all duration-300 border border-blue-200/30">
                        <div class="flex items-start gap-4 sm:gap-5">
                            <div
                                class="flex-shrink-0 w-12 h-12 sm:w-14 sm:h-14 rounded-xl sm:rounded-2xl bg-gradient-to-br from-blue-500 to-cyan-400 flex items-center justify-center shadow-lg shadow-blue-500/25 group-hover:scale-110 transition-transform">
                                <svg class="w-6 h-6 sm:w-7 sm:h-7 text-white" fill="none" stroke="currentColor"
                                    viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                                </svg>
                            </div>
                            <div class="flex-1">
                                <h3 class="text-lg sm:text-xl font-bold text-gray-900 mb-3 sm:mb-4">Jam Operasional</h3>
                                <div class="space-y-2 sm:space-y-3">
                                    <div class="flex justify-between items-center py-2 border-b border-gray-200/50">
                                        <span class="text-gray-700 font-medium text-sm sm:text-base">Senin –
                                            Jumat</span>
                                        <span class="text-blue-500 font-semibold text-sm sm:text-base">07.00 –
                                            22.00</span>
                                    </div>
                                    <div class="flex justify-between items-center py-2 border-b border-gray-200/50">
                                        <span class="text-gray-700 font-medium text-sm sm:text-base">Sabtu &
                                            Minggu</span>
                                        <span class="text-blue-500 font-semibold text-sm sm:text-base">08.00 –
                                            21.00</span>
                                    </div>
                                    <div class="flex justify-between items-center py-2">
                                        <span class="text-gray-700 font-medium text-sm sm:text-base">Antar-Jemput</span>
                                        <span class="text-green-600 font-semibold text-sm sm:text-base">24/7
                                            Available</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Right Column - Mobile Phone Mockup -->
                <div class="flex justify-center lg:justify-end lg:sticky lg:top-8">
                    <div class="relative w-full max-w-[300px] sm:max-w-[320px]">
                        <div
                            class="absolute -inset-3 sm:-inset-4 bg-gradient-to-r from-blue-400/20 to-cyan-300/20 rounded-[3rem] sm:rounded-[4rem] blur-2xl opacity-60">
                        </div>
                        <div
                            class="relative w-full aspect-[9/19] rounded-[2.5rem] sm:rounded-[3rem] bg-gradient-to-br from-gray-900 to-gray-800 shadow-2xl p-2 border overflow-hidden">
                            <!-- Notch -->
                            <div
                                class="absolute mt-2 left-1/2 -translate-x-1/2 w-24 sm:w-30 h-6 sm:h-7 bg-black rounded-3xl z-20 flex items-end justify-center pb-1">
                                <div class="w-12 sm:w-16 h-1 bg-gray-800 rounded-full"></div>
                            </div>

                            <!-- Screen Content -->
                            <div
                                class="w-full h-full rounded-[2rem] sm:rounded-[2.3rem] overflow-hidden bg-white relative">
                                <!-- Location Card Overlay -->
                                <div class="absolute bottom-16 sm:bottom-20 left-0 right-0 z-10 px-3 sm:px-4">
                                    <div class="flex items-center justify-between bg-white p-2 rounded-xl shadow-lg">
                                        <div class="flex items-center gap-2 sm:gap-3">
                                            <div
                                                class="w-8 h-8 sm:w-10 sm:h-10 rounded-lg sm:rounded-xl bg-blue-500 flex items-center justify-center shadow-lg flex-shrink-0">
                                                <svg class="w-4 h-4 sm:w-5 sm:h-5 text-white" fill="none"
                                                    stroke="currentColor" viewBox="0 0 24 24">
                                                    <path stroke-linecap="round" stroke-linejoin="round"
                                                        stroke-width="2"
                                                        d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z">
                                                    </path>
                                                    <path stroke-linecap="round" stroke-linejoin="round"
                                                        stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path>
                                                </svg>
                                            </div>
                                            <div class="min-w-0">
                                                <p class="text-xs sm:text-sm font-bold text-gray-900 truncate">Laundry
                                                    Express</p>
                                                <p class="text-xs text-gray-500 truncate">Jl. Jepara Kedung No. 12</p>
                                            </div>
                                        </div>
                                    </div>
                                </div>

                                <!-- Google Maps Embed -->
                                <iframe class="w-full h-full border-0" loading="lazy"
                                    referrerpolicy="no-referrer-when-downgrade"
                                    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3960.8985!2d110.6633!3d-6.5892!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zNsKwMzUnMjEuMSJTIDExMMKwMzknNDcuOSJF!5e0!3m2!1sen!2sid!4v1234567890"></iframe>

                                <!-- Bottom CTA -->
                                <div
                                    class="absolute bottom-0 left-0 right-0 p-3 sm:p-4 bg-gradient-to-t from-white via-white to-transparent">
                                    <button
                                        class="w-full py-2.5 sm:py-3 bg-gradient-to-r from-blue-500 to-cyan-400 text-white rounded-xl font-semibold shadow-lg flex items-center justify-center gap-2 hover:shadow-xl transition-all text-sm sm:text-base">
                                        <svg class="w-4 h-4 sm:w-5 sm:h-5" fill="none" stroke="currentColor"
                                            viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                                d="M9 20l-5.447-2.724A1 1 0 013 16.382V5.618a1 1 0 011.447-.894L9 7m0 13l6-3m-6 3V7m6 10l4.553 2.276A1 1 0 0021 18.382V7.618a1 1 0 00-.553-.894L15 4m0 13V4m0 0L9 7">
                                            </path>
                                        </svg>
                                        Buka di Maps
                                    </button>
                                </div>
                            </div>

                            <!-- Phone Buttons -->
                            <div class="absolute right-0 top-20 sm:top-28 w-1 h-10 sm:h-12 bg-gray-700 rounded-l-lg">
                            </div>
                            <div class="absolute right-0 top-32 sm:top-44 w-1 h-12 sm:h-16 bg-gray-700 rounded-l-lg">
                            </div>
                            <div class="absolute right-0 top-48 sm:top-64 w-1 h-12 sm:h-16 bg-gray-700 rounded-l-lg">
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style>
@keyframes float {

    0%,
    100% {
        transform: translateY(0px) rotate(45deg);
    }

    50% {
        transform: translateY(-20px) rotate(45deg);
    }
}

@keyframes spin-slow {
    0% {
        transform: rotate(0deg);
    }

    100% {
        transform: rotate(360deg);
    }
}

.animate-float {
    animation: float 6s ease-in-out infinite;
}

.animate-spin-slow {
    animation: spin-slow 20s linear infinite;
}
</style>