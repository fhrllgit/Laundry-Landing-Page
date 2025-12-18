<template>
    <div class="w-full min-h-screen relative overflow-hidden bg-gradient-to-br from-white via-blue-50 to-cyan-50">
        <!-- Grid Pattern Background -->
        <div class="absolute inset-0 opacity-[0.03]">
            <div class="absolute inset-0" style="background-image: linear-gradient(#2196f3 1px, transparent 1px), linear-gradient(90deg, #2196f3 1px, transparent 1px); background-size: 50px 50px;"></div>
        </div>
        
        <!-- Floating Decorative Elements -->
        <div class="absolute top-20 left-10 w-72 h-72 bg-blue-200 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-blob"></div>
        <div class="absolute top-40 right-10 w-72 h-72 bg-cyan-200 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-blob animation-delay-2000"></div>
        <div class="absolute -bottom-8 left-20 w-72 h-72 bg-blue-300 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-blob animation-delay-4000"></div>
        
        <div class="flex flex-col lg:flex-row md:px-10 px-5 lg:px-40 w-full justify-center items-center min-h-screen relative z-10 py-20 gap-12">
            <!-- Left Content -->
            <div class="flex-1 flex flex-col space-y-6 lg:space-y-8">
                <div class="flex space-y-3 flex-col">
                    <h1 class="text-4xl md:text-5xl lg:text-6xl leading-tight" style="font-weight: 800;">Laundry</h1>
                    <p class="text-4xl md:text-5xl lg:text-6xl bg-gradient-to-r from-[#2196f3] via-[#34c1dd] to-[#2196f3] bg-clip-text text-transparent leading-tight"
                        style="font-weight: 800;">Bersih, Wangi</p>
                    <p class="text-4xl md:text-5xl lg:text-6xl bg-gradient-to-r from-[#2196f3] via-[#34c1dd] to-[#2196f3] bg-clip-text text-transparent leading-tight"
                        style="font-weight: 800;">dan Tepat Waktu</p>
                </div>
                <p class="text-base md:text-lg text-[#646363] max-w-xl leading-relaxed">
                    Kami hadir untuk merawat pakaian Anda dengan teknologi modern dan tenaga profesional. Bersih maksimal, wangi tahan lama, tanpa ribet.
                </p>
                
                <!-- Stats -->
                <div class="flex gap-6 md:gap-8 flex-wrap">
                    <div class="flex flex-col">
                        <span class="text-3xl md:text-4xl font-bold text-[#2196f3]">500+</span>
                        <span class="text-sm text-[#646363]">Pelanggan Puas</span>
                    </div>
                    <div class="flex flex-col">
                        <span class="text-3xl md:text-4xl font-bold text-[#2196f3]">24 Jam</span>
                        <span class="text-sm text-[#646363]">Layanan Express</span>
                    </div>
                    <div class="flex flex-col">
                        <span class="text-3xl md:text-4xl font-bold text-[#2196f3]">100%</span>
                        <span class="text-sm text-[#646363]">Garansi Bersih</span>
                    </div>
                </div>
                
                <div class="flex items-center gap-4 flex-wrap">
                    <div class="flex items-center gap-2 px-5 py-3 rounded-xl cursor-pointer bg-gradient-to-r from-[#2196f3] to-[#34c1dd] w-max shadow-lg hover:shadow-xl transition-all duration-300 hover:scale-105 group">
                        <span class="text-white font-semibold">Pesan Sekarang</span>
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2"
                            stroke="currentColor" class="size-5 text-white group-hover:translate-x-1 transition-transform">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M17.25 8.25 21 12m0 0-3.75 3.75M21 12H3" />
                        </svg>
                    </div>
                    <button class="px-5 py-3 rounded-xl border-2 border-[#2196f3] text-[#2196f3] font-semibold hover:bg-[#2196f3] hover:text-white transition-all duration-300">
                        Lihat Harga
                    </button>
                </div>
            </div>
            
            <!-- Right Image Section -->
            <div class="flex-1 relative">
                <!-- Decorative Grid Background -->
                <div class="absolute inset-0 -z-10">
                    <div class="absolute top-0 right-0 w-80 h-80 bg-gradient-to-br from-blue-400/20 to-cyan-400/20 rounded-3xl rotate-12 blur-2xl"></div>
                    <div class="absolute bottom-0 left-0 w-64 h-64 bg-gradient-to-tr from-cyan-400/20 to-blue-400/20 rounded-3xl -rotate-12 blur-2xl"></div>
                </div>
                
                <!-- Main Image Container -->
                <div class="relative">
                    <!-- Grid Pattern Card -->
                    <div class="absolute -inset-4 bg-white/40 backdrop-blur-sm rounded-3xl" style="background-image: linear-gradient(rgba(33, 150, 243, 0.05) 1px, transparent 1px), linear-gradient(90deg, rgba(33, 150, 243, 0.05) 1px, transparent 1px); background-size: 20px 20px;"></div>
                    
                    <!-- Image Grid -->
                    <div class="relative grid grid-cols-2 gap-4 p-4">
                        <!-- Top Left - Washing Machine -->
                        <div class="col-span-2 bg-white rounded-2xl shadow-xl overflow-hidden hover:shadow-2xl transition-all duration-300 hover:scale-[1.02]">
                            <img src="https://images.unsplash.com/photo-1582735689369-4fe89db7114c?w=800&q=80" 
                                 alt="Mesin Cuci Modern" 
                                 class="w-full h-64 object-cover">
                        </div>
                        
                        <!-- Bottom Left - Water Splash Effect -->
                        <div class="bg-gradient-to-br from-blue-100 to-cyan-100 rounded-2xl shadow-lg overflow-hidden hover:shadow-xl transition-all duration-300 hover:scale-[1.02] p-6 flex items-center justify-center">
                            <div class="text-center">
                                <div class="w-16 h-16 mx-auto mb-3 bg-white rounded-full flex items-center justify-center shadow-lg">
                                    <svg class="w-8 h-8 text-[#2196f3]" fill="currentColor" viewBox="0 0 20 20">
                                        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm1-11a1 1 0 10-2 0v3.586L7.707 9.293a1 1 0 00-1.414 1.414l3 3a1 1 0 001.414 0l3-3a1 1 0 00-1.414-1.414L11 10.586V7z" clip-rule="evenodd"/>
                                    </svg>
                                </div>
                                <p class="text-sm font-semibold text-[#2196f3]">Teknologi Modern</p>
                            </div>
                        </div>
                        
                        <!-- Bottom Right - Clean Clothes -->
                        <div class="bg-gradient-to-br from-cyan-100 to-blue-100 rounded-2xl shadow-lg overflow-hidden hover:shadow-xl transition-all duration-300 hover:scale-[1.02] p-6 flex items-center justify-center">
                            <div class="text-center">
                                <div class="w-16 h-16 mx-auto mb-3 bg-white rounded-full flex items-center justify-center shadow-lg">
                                    <svg class="w-8 h-8 text-[#34c1dd]" fill="currentColor" viewBox="0 0 20 20">
                                        <path d="M9 2a1 1 0 000 2h2a1 1 0 100-2H9z"/>
                                        <path fill-rule="evenodd" d="M4 5a2 2 0 012-2 3 3 0 003 3h2a3 3 0 003-3 2 2 0 012 2v11a2 2 0 01-2 2H6a2 2 0 01-2-2V5zm9.707 5.707a1 1 0 00-1.414-1.414L9 12.586l-1.293-1.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
                                    </svg>
                                </div>
                                <p class="text-sm font-semibold text-[#34c1dd]">Garansi Bersih</p>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Floating Badge -->
                    <div class="absolute -top-4 -right-4 bg-white rounded-full p-4 shadow-xl animate-bounce-slow">
                        <div class="text-center">
                            <p class="text-2xl font-bold text-[#2196f3]">⭐</p>
                            <p class="text-xs font-semibold text-[#646363]">4.9/5.0</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
@keyframes blob {
  0% {
    transform: translate(0px, 0px) scale(1);
  }
  33% {
    transform: translate(30px, -50px) scale(1.1);
  }
  66% {
    transform: translate(-20px, 20px) scale(0.9);
  }
  100% {
    transform: translate(0px, 0px) scale(1);
  }
}

.animate-blob {
  animation: blob 7s infinite;
}

.animation-delay-2000 {
  animation-delay: 2s;
}

.animation-delay-4000 {
  animation-delay: 4s;
}

@keyframes bounce-slow {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-10px);
  }
}

.animate-bounce-slow {
  animation: bounce-slow 3s ease-in-out infinite;
}
</style>