<template>
    <div class="w-full min-h-screen relative overflow-hidden">
        <div class="absolute inset-0 flex items-center justify-center pointer-events-none">
            <div
                class="absolute right-1/2 mr-10 mb-30 w-20 h-20 lg:w-28 lg:h-28 border-2 border-[#34c1dd]/20 rounded-2xl -rotate-12 animate-float-delay">
            </div>
            <div
                class="absolute top-0 mt-25 left-0 w-16 h-16 lg:w-24 lg:h-24 border-2 border-[#2196f3]/15 rounded-xl rotate-45 animate-float-delay-2">
            </div>
        </div>
        <div
            class="flex flex-col lg:flex-row md:px-10 px-5 lg:px-40 w-full justify-center items-center min-h-screen py-20 lg:py-0 gap-12 lg:gap-16">
            <div class="flex-1 relative flex flex-col space-y-6 lg:space-y-8 z-10 w-full">
                <div class="flex flex-col space-y-3">
                    <h1 class="text-4xl md:text-5xl lg:text-6xl leading-tight animate-fade-in font-extrabold">
                        Laundry
                    </h1>
                    <p
                        class="text-4xl md:text-5xl lg:text-6xl bg-gradient-to-r from-[#2196f3] via-[#34c1dd] to-[#2196f3] bg-clip-text text-transparent leading-tight animate-fade-in-delay font-extrabold">
                        Bersih, Wangi
                    </p>
                    <p
                        class="text-4xl md:text-5xl lg:text-6xl bg-gradient-to-r from-[#2196f3] via-[#34c1dd] to-[#2196f3] bg-clip-text text-transparent leading-tight animate-fade-in-delay-2 font-extrabold">
                        dan Tepat Waktu
                    </p>
                </div>
                <p class="text-base md:text-lg text-[#646363] leading-relaxed max-w-xl">
                    Kami hadir untuk merawat pakaian Anda dengan teknologi modern dan tenaga profesional. Bersih
                    maksimal, wangi tahan lama, tanpa ribet.
                </p>
                <div class="flex gap-6 md:gap-8 flex-wrap">
                    <div class="flex flex-col">
                        <span
                            class="text-3xl md:text-4xl font-bold bg-gradient-to-r from-[#2196f3] to-[#34c1dd] bg-clip-text text-transparent">500+</span>
                        <span class="text-sm text-[#646363]">Pelanggan Puas</span>
                    </div>
                    <div class="flex flex-col">
                        <span
                            class="text-3xl md:text-4xl font-bold bg-gradient-to-r from-[#2196f3] to-[#34c1dd] bg-clip-text text-transparent">24
                            Jam</span>
                        <span class="text-sm text-[#646363]">Layanan Express</span>
                    </div>
                    <div class="flex flex-col">
                        <span
                            class="text-3xl md:text-4xl font-bold bg-gradient-to-r from-[#2196f3] to-[#34c1dd] bg-clip-text text-transparent">100%</span>
                        <span class="text-sm text-[#646363]">Garansi Bersih</span>
                    </div>
                </div>
                <div class="flex items-center gap-4 flex-wrap">
                    <div
                        class="flex items-center gap-2 px-5 py-3 rounded-xl cursor-pointer bg-gradient-to-r from-[#2196f3] to-[#34c1dd] w-max shadow-lg hover:shadow-xl transition-all duration-300 hover:scale-105 group">
                        <span class="text-white font-semibold">Pesan Sekarang</span>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2"
                            stroke="currentColor"
                            class="w-5 h-5 text-white group-hover:translate-x-1 transition-transform duration-300">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M17.25 8.25 21 12m0 0-3.75 3.75M21 12H3" />
                        </svg>
                    </div>
                    <button
                        class="px-5 py-3 rounded-xl border-2 border-[#2196f3] text-[#2196f3] font-semibold hover:bg-[#2196f3] hover:text-white transition-all duration-300">
                        Lihat Harga
                    </button>
                </div>
            </div>
            <div class="flex-1 flex items-center justify-center relative w-full">
                <div class="absolute inset-0 flex items-center justify-center pointer-events-none">
                    <div
                        class="absolute right-0 bottom-0 w-24 h-24 lg:w-32 lg:h-32 border-2 border-[#2196f3]/20 rounded-2xl rotate-12 animate-float">
                    </div>
                    <div
                        class="absolute -top-10 -right-10 w-40 h-40 lg:w-64 lg:h-64 bg-gradient-to-br from-blue-300/20 to-transparent rounded-full blur-3xl animate-pulse-slow">
                    </div>
                    <div
                        class="absolute -bottom-10 -left-10 w-40 h-40 lg:w-64 lg:h-64 bg-gradient-to-tr from-cyan-300/20 to-transparent rounded-full blur-3xl animate-pulse-slow-delay">
                    </div>
                    <div class="water-bubble" style="top:15%; left:10%;"></div>
                    <div class="water-bubble" style="top:45%; right:15%; animation-delay:1s;"></div>
                    <div class="water-bubble" style="bottom:20%; left:20%; animation-delay:2s;"></div>
                </div>
                <div class="relative z-10 w-full max-w-md lg:max-w-lg">
                    <div class="bg-white/80 backdrop-blur-sm shadow-xl rounded-2xl lg:rounded-3xl overflow-hidden">
                        <div
                            class="rounded-2xl lg:rounded-3xl overflow-hidden transform hover:scale-[1.02] transition-all duration-500 hover:shadow-[#2196f3]/20 hover:shadow-3xl">
                            <img class="w-full h-auto object-cover" src="../../assets/img/contentImage.jpg"
                                alt="Laundry Service" />
                        </div>
                    </div>
                    <div
                        class="absolute -bottom-4 -left-4 bg-gradient-to-r from-[#2196f3] to-[#34c1dd] rounded-2xl p-4 shadow-xl z-20">
                        <div class="flex items-center gap-2">
                            <div class="w-10 h-10 bg-white/20 rounded-full flex items-center justify-center">
                                <svg class="w-5 h-5 text-white" fill="currentColor" viewBox="0 0 20 20">
                                    <path fill-rule="evenodd"
                                        d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z"
                                        clip-rule="evenodd" />
                                </svg>
                            </div>
                            <div>
                                <p class="text-white font-bold text-sm">Garansi</p>
                                <p class="text-white/80 text-xs">100% Bersih</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped>
@keyframes float {

    0%,
    100% {
        transform: translateY(0) rotate(12deg);
    }

    50% {
        transform: translateY(-20px) rotate(12deg);
    }
}

@keyframes float-delay {

    0%,
    100% {
        transform: translateY(0) rotate(-12deg);
    }

    50% {
        transform: translateY(-15px) rotate(-12deg);
    }
}

@keyframes float-delay-2 {

    0%,
    100% {
        transform: translateY(0) rotate(45deg);
    }

    50% {
        transform: translateY(-25px) rotate(45deg);
    }
}

@keyframes bubble {
    0% {
        transform: translateY(0) scale(0);
        opacity: 0;
    }

    50% {
        opacity: 1;
    }

    100% {
        transform: translateY(-100px) scale(1);
        opacity: 0;
    }
}

@keyframes pulse-slow {

    0%,
    100% {
        opacity: 0.3;
        transform: scale(1);
    }

    50% {
        opacity: 0.5;
        transform: scale(1.1);
    }
}

@keyframes fade-in {
    from {
        opacity: 0;
        transform: translateY(20px);
    }

    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.animate-float {
    animation: float 6s ease-in-out infinite;
}

.animate-float-delay {
    animation: float-delay 7s ease-in-out infinite;
    animation-delay: 1s;
}

.animate-float-delay-2 {
    animation: float-delay-2 8s ease-in-out infinite;
    animation-delay: 2s;
}

.animate-pulse-slow {
    animation: pulse-slow 4s ease-in-out infinite;
}

.animate-pulse-slow-delay {
    animation: pulse-slow 5s ease-in-out infinite;
    animation-delay: 2s;
}

.animate-fade-in {
    animation: fade-in 1s ease-out;
}

.animate-fade-in-delay {
    animation: fade-in 1s ease-out 0.2s backwards;
}

.animate-fade-in-delay-2 {
    animation: fade-in 1s ease-out 0.4s backwards;
}

.water-bubble {
    position: absolute;
    width: 8px;
    height: 8px;
    background: radial-gradient(circle, #2196f3, #34c1dd);
    border-radius: 50%;
    opacity: 0.6;
    animation: bubble 4s ease-in-out infinite;
}

@media (max-width:1024px) {
    .water-bubble {
        width: 6px;
        height: 6px;
    }
}
</style>
