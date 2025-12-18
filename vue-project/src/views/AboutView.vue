<template>
  <section class="px-5 md:px-10 lg:px-20 xl:px-40 py-16 md:py-20 bg-white">
    <!-- Header Section -->
    <div class="text-center mb-12 md:mb-16">
      <p class="text-[#2196F3] font-semibold text-sm md:text-base mb-2 uppercase tracking-wide">
        Testimonial
      </p>
      <h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900 mb-3">
        Apa Kata Pelanggan
      </h2>
      <p class="text-gray-600 text-base md:text-lg max-w-2xl mx-auto">
        Kepercayaan pelanggan adalah prioritas kami
      </p>
    </div>

    <!-- Testimonials Slider Container -->
    <div class="relative">
      <!-- Slider Wrapper -->
      <div
        ref="sliderRef"
        class="flex gap-6 overflow-x-auto scrollbar-hide scroll-smooth snap-x snap-mandatory pb-4"
        @scroll="updateNavButtons"
      >
        <!-- Testimonial Card -->
        <div
          v-for="testimonial in testimonials"
          :key="testimonial.id"
          class="flex-shrink-0 w-full md:w-[calc(50%-12px)] lg:w-[calc(33.333%-16px)] snap-start"
        >
          <div class="bg-white rounded-2xl shadow-lg hover:shadow-xl transition-shadow duration-300 p-6 md:p-8 h-full border border-gray-100">
            <!-- Rating Stars -->
            <div class="flex gap-1 mb-4">
              <svg
                v-for="star in 5"
                :key="star"
                class="w-5 h-5"
                :class="star <= testimonial.rating ? 'text-[#2196F3]' : 'text-gray-300'"
                fill="currentColor"
                viewBox="0 0 20 20"
              >
                <path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z" />
              </svg>
            </div>

            <!-- Testimonial Text -->
            <p class="text-gray-700 text-base md:text-lg leading-relaxed mb-6 italic">
              "{{ testimonial.comment }}"
            </p>

            <!-- Customer Info -->
            <div class="flex items-center gap-4 mt-auto">
              <!-- Avatar -->
              <div class="w-12 h-12 rounded-full bg-gradient-to-br from-[#2196F3] to-[#1976D2] flex items-center justify-center text-white font-bold text-lg flex-shrink-0">
                {{ testimonial.initials }}
              </div>
              
              <!-- Name & Role -->
              <div>
                <h4 class="font-semibold text-gray-900 text-base md:text-lg">
                  {{ testimonial.name }}
                </h4>
                <p class="text-gray-500 text-sm">
                  {{ testimonial.location }}
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Navigation Buttons -->
      <div class="flex gap-3 justify-end mt-8">
        <!-- Previous Button -->
        <button
          ref="prevBtn"
          @click="scrollPrev"
          :disabled="isAtStart"
          class="w-12 h-12 rounded-full bg-[#2196F3] hover:bg-[#1976D2] disabled:bg-gray-300 disabled:cursor-not-allowed text-white flex items-center justify-center transition-all duration-300 shadow-md hover:shadow-lg transform hover:scale-105 active:scale-95"
          aria-label="Previous testimonial"
        >
          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
          </svg>
        </button>

        <!-- Next Button -->
        <button
          ref="nextBtn"
          @click="scrollNext"
          :disabled="isAtEnd"
          class="w-12 h-12 rounded-full bg-[#2196F3] hover:bg-[#1976D2] disabled:bg-gray-300 disabled:cursor-not-allowed text-white flex items-center justify-center transition-all duration-300 shadow-md hover:shadow-lg transform hover:scale-105 active:scale-95"
          aria-label="Next testimonial"
        >
          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
          </svg>
        </button>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from 'vue';

const sliderRef = ref(null);
const isAtStart = ref(true);
const isAtEnd = ref(false);

const testimonials = [
  {
    id: 1,
    name: 'Rina Susanti',
    initials: 'RS',
    location: 'Jakarta Selatan',
    rating: 5,
    comment: 'Pelayanan sangat memuaskan! Pakaian saya bersih wangi dan rapi. Proses pengantaran juga tepat waktu. Sangat recommend untuk yang sibuk seperti saya.'
  },
  {
    id: 2,
    name: 'Budi Hartono',
    initials: 'BH',
    location: 'Bandung',
    rating: 5,
    comment: 'Sudah langganan 6 bulan, belum pernah kecewa. Harga terjangkau, hasil maksimal. Customer service nya juga ramah dan responsif banget.'
  },
  {
    id: 3,
    name: 'Siti Nurhaliza',
    initials: 'SN',
    location: 'Surabaya',
    rating: 4,
    comment: 'Kualitas cucian bagus dan wanginya tahan lama. Aplikasinya juga user-friendly, memudahkan untuk tracking order. Puas dengan layanannya!'
  },
  {
    id: 4,
    name: 'Ahmad Rizki',
    initials: 'AR',
    location: 'Depok',
    rating: 5,
    comment: 'Laundry terbaik yang pernah saya coba! Kemeja kerja saya selalu rapi dan harum. Delivery driver nya juga profesional dan tepat waktu.'
  },
  {
    id: 5,
    name: 'Dewi Kartika',
    initials: 'DK',
    location: 'Tangerang',
    rating: 5,
    comment: 'Sangat membantu saya yang sibuk bekerja. Tinggal order lewat aplikasi, dijemput, dan diantar kembali. Hasilnya selalu memuaskan!'
  },
  {
    id: 6,
    name: 'Eko Prasetyo',
    initials: 'EP',
    location: 'Bekasi',
    rating: 4,
    comment: 'Harga kompetitif dengan kualitas premium. Paket berlangganan nya juga worth it banget. Terima kasih sudah memudahkan hidup saya!'
  }
];

const scrollPrev = () => {
  if (sliderRef.value) {
    const scrollAmount = sliderRef.value.offsetWidth;
    sliderRef.value.scrollBy({
      left: -scrollAmount,
      behavior: 'smooth'
    });
  }
};

const scrollNext = () => {
  if (sliderRef.value) {
    const scrollAmount = sliderRef.value.offsetWidth;
    sliderRef.value.scrollBy({
      left: scrollAmount,
      behavior: 'smooth'
    });
  }
};

const updateNavButtons = () => {
  if (sliderRef.value) {
    const { scrollLeft, scrollWidth, clientWidth } = sliderRef.value;
    isAtStart.value = scrollLeft <= 10;
    isAtEnd.value = scrollLeft + clientWidth >= scrollWidth - 10;
  }
};

onMounted(() => {
  updateNavButtons();
  if (sliderRef.value) {
    sliderRef.value.addEventListener('scroll', updateNavButtons);
  }
});
</script>

<style scoped>
/* Hide scrollbar but keep functionality */
.scrollbar-hide {
  -ms-overflow-style: none;
  scrollbar-width: none;
}

.scrollbar-hide::-webkit-scrollbar {
  display: none;
}

/* Smooth scroll behavior */
.scroll-smooth {
  scroll-behavior: smooth;
}

/* Snap scroll alignment */
.snap-x {
  scroll-snap-type: x mandatory;
}

.snap-start {
  scroll-snap-align: start;
}

/* Additional smooth animations */
@media (prefers-reduced-motion: no-preference) {
  .transition-all {
    transition-property: all;
    transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  }
}
</style>