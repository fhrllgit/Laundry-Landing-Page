<template>
    <footer class="bg-white border-t border-gray-100">
        <div class="px-5 md:px-10 lg:px-20 xl:px-40 py-12 md:py-16">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8 md:gap-12">
                <div class="space-y-4">
                    <div class="flex items-center space-x-3">
                        <div class="w-10 h-10 bg-blue-50 rounded-xl flex items-center justify-center">
                            <svg class="w-6 h-6 text-[#2196F3]" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                    d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10" />
                            </svg>
                        </div>
                        <h3 class="text-xl font-bold text-gray-800">ZahraLaundry</h3>
                    </div>
                    <p class="text-gray-600 text-sm leading-relaxed">
                        Layanan laundry modern dengan kualitas terbaik. Cepat, bersih, dan terpercaya
                        untuk kebutuhan cucian Anda.
                    </p>
                    <div class="flex items-center space-x-3 pt-2">
                        <a v-for="social in socialMedia" :key="social.name" :href="social.href" target="_blank"
                            rel="noopener noreferrer"
                            class="w-9 h-9 bg-gray-50 rounded-lg flex items-center justify-center transition-all duration-300 hover:bg-[#2196F3] hover:shadow-md group"
                            :aria-label="social.name">
                            <component :is="social.icon"
                                class="w-4 h-4 text-gray-600 group-hover:text-white transition-colors" />
                        </a>
                    </div>
                </div>
                <div class="space-y-4">
                    <h4 class="text-lg font-semibold text-gray-800">Menu</h4>
                    <ul class="space-y-3">
                        <li v-for="item in menuItems" :key="item.id">
                            <a :href="item.href"
                                class="text-gray-600 text-sm hover:text-[#2196F3] transition-colors duration-300 inline-block hover:translate-x-1 transform">
                                {{ item.name }}
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="space-y-4">
                    <h4 class="text-lg font-semibold text-gray-800">Kontak</h4>

                    <div class="space-y-3">
                        <a href="tel:+6281234567890"
                            class="flex items-start space-x-3 text-gray-600 hover:text-[#2196F3] transition-colors group">
                            <Phone class="w-5 h-5 mt-0.5 group-hover:scale-110 transition-transform" />
                            <span class="text-sm">+62 812-3456-7890</span>
                        </a>

                        <a href="mailto:info@laundrykita.com"
                            class="flex items-start space-x-3 text-gray-600 hover:text-[#2196F3] transition-colors group">
                            <Mail class="w-5 h-5 mt-0.5 group-hover:scale-110 transition-transform" />
                            <span class="text-sm">info@laundrykita.com</span>
                        </a>

                        <div class="flex items-start space-x-3 text-gray-600">
                            <MapPin class="w-5 h-5 mt-0.5" />
                            <span class="text-sm">
                                Jl. Nalumsari No. 123<br />
                                Jepara Selatan, 12345
                            </span>
                        </div>
                    </div>
                </div>
                <div class="space-y-4">
                    <h4 class="text-lg font-semibold text-gray-800">Hubungi Kami</h4>
                    <p class="text-gray-600 text-sm">
                        Ada pertanyaan? Chat dengan kami sekarang!
                    </p>

                    <button @click="handleWhatsApp"
                        class="w-full cursor-pointer bg-[#2196F3] text-white px-6 py-3 rounded-xl font-medium text-sm flex items-center justify-center space-x-2 hover:bg-[#1976D2] transition-all duration-300 shadow-md hover:shadow-lg transform hover:-translate-y-0.5">
                        <svg class="size-5 text-white" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"
                            fill="currentColor">
                            <path
                                d="M12.001 2C17.5238 2 22.001 6.47715 22.001 12C22.001 17.5228 17.5238 22 12.001 22C10.1671 22 8.44851 21.5064 6.97086 20.6447L2.00516 22L3.35712 17.0315C2.49494 15.5536 2.00098 13.8345 2.00098 12C2.00098 6.47715 6.47813 2 12.001 2ZM8.59339 7.30019L8.39232 7.30833C8.26293 7.31742 8.13607 7.34902 8.02057 7.40811C7.93392 7.45244 7.85348 7.51651 7.72709 7.63586C7.60774 7.74855 7.53857 7.84697 7.46569 7.94186C7.09599 8.4232 6.89729 9.01405 6.90098 9.62098C6.90299 10.1116 7.03043 10.5884 7.23169 11.0336C7.63982 11.9364 8.31288 12.8908 9.20194 13.7759C9.4155 13.9885 9.62473 14.2034 9.85034 14.402C10.9538 15.3736 12.2688 16.0742 13.6907 16.4482C13.6907 16.4482 14.2507 16.5342 14.2589 16.5347C14.4444 16.5447 14.6296 16.5313 14.8153 16.5218C15.1066 16.5068 15.391 16.428 15.6484 16.2909C15.8139 16.2028 15.8922 16.159 16.0311 16.0714C16.0311 16.0714 16.0737 16.0426 16.1559 15.9814C16.2909 15.8808 16.3743 15.81 16.4866 15.6934C16.5694 15.6074 16.6406 15.5058 16.6956 15.3913C16.7738 15.2281 16.8525 14.9166 16.8838 14.6579C16.9077 14.4603 16.9005 14.3523 16.8979 14.2854C16.8936 14.1778 16.8047 14.0671 16.7073 14.0201L16.1258 13.7587C16.1258 13.7587 15.2563 13.3803 14.7245 13.1377C14.6691 13.1124 14.6085 13.1007 14.5476 13.097C14.4142 13.0888 14.2647 13.1236 14.1696 13.2238C14.1646 13.2218 14.0984 13.279 13.3749 14.1555C13.335 14.2032 13.2415 14.3069 13.0798 14.2972C13.0554 14.2955 13.0311 14.292 13.0074 14.2858C12.9419 14.2685 12.8781 14.2457 12.8157 14.2193C12.692 14.1668 12.6486 14.1469 12.5641 14.1105C11.9868 13.8583 11.457 13.5209 10.9887 13.108C10.8631 12.9974 10.7463 12.8783 10.6259 12.7616C10.2057 12.3543 9.86169 11.9211 9.60577 11.4938C9.5918 11.4705 9.57027 11.4368 9.54708 11.3991C9.50521 11.331 9.45903 11.25 9.44455 11.1944C9.40738 11.0473 9.50599 10.9291 9.50599 10.9291C9.50599 10.9291 9.74939 10.663 9.86248 10.5183C9.97128 10.379 10.0652 10.2428 10.125 10.1457C10.2428 9.95633 10.2801 9.76062 10.2182 9.60963C9.93764 8.92565 9.64818 8.24536 9.34986 7.56894C9.29098 7.43545 9.11585 7.33846 8.95659 7.32007C8.90265 7.31384 8.84875 7.30758 8.79459 7.30402C8.66053 7.29748 8.5262 7.29892 8.39232 7.30833L8.59339 7.30019Z">
                            </path>
                        </svg>
                        <span>Chat WhatsApp</span>
                    </button>

                    <div class="bg-blue-50 rounded-xl p-4 mt-4">
                        <p class="text-xs text-gray-600 text-center">
                            <span class="font-semibold text-[#2196F3]">Buka:</span> Senin - Sabtu<br />
                            08:00 - 20:00 WIB
                        </p>
                    </div>
                </div>
            </div>
            <div class="border-t border-gray-100 mt-12 pt-8">
                <div class="flex flex-col md:flex-row justify-between items-center gap-4">
                    <p class="text-sm text-gray-500 text-center md:text-left">
                        © {{ year }} ZahraLaundry. All rights reserved.
                    </p>
                    <div class="flex items-center space-x-6">
                        <a href="#" class="text-sm text-gray-500 hover:text-[#2196F3] transition-colors">
                            Syarat & Ketentuan
                        </a>
                        <a href="#" class="text-sm text-gray-500 hover:text-[#2196F3] transition-colors">
                            Kebijakan Privasi
                        </a>
                    </div>
                </div>
            </div>

        </div>
    </footer>
</template>

<script setup>
import {
    MapPin,
    Phone,
    Mail,
    MessageCircle,
    Instagram,
    Facebook
} from 'lucide-vue-next'
import Swal from 'sweetalert2'


const year = new Date().getFullYear()

const menuItems = [
    { id: 1, name: 'Beranda', href: '#' },
    { id: 2, name: 'Jasa', href: '#jasa' },
    { id: 3, name: 'Harga', href: '#harga' },
    { id: 4, name: 'Kontak', href: '#kontak' }
]

const socialMedia = [
    { name: 'WhatsApp', icon: MessageCircle, href: 'https://wa.me/6281234567890' },
    { name: 'Instagram', icon: Instagram, href: 'https://instagram.com/laundrykita' },
    { name: 'Facebook', icon: Facebook, href: 'https://facebook.com/laundrykita' }
]

const handleWhatsApp = () => {
    Swal.fire({
        icon: 'info',
        title: 'Fitur Belum Tersedia',
        text: 'Mohon maaf, fitur ini sedang dalam tahap pengembangan.',
        confirmButtonText: 'Mengerti',
        confirmButtonColor: '#2196F3',
        background: '#fff',
        color: '#1f2937',
        showClass: {
            popup: 'animate__animated animate__fadeInDown'
        },
        hideClass: {
            popup: 'animate__animated animate__fadeOutUp'
        }
    })
}
</script>
