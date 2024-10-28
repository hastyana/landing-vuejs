<template>
    <div class="brand-slider overflow-hidden">
      <div
        class="d-flex brand-track"
        :style="{ transform: `translateX(-${currentOffset}px)`, transition: 'transform 1s ease' }"
      >
        <div v-for="(brand, index) in brands" :key="index" class="brand-item">
          <img :src="brand.logo" :alt="brand.name" class="img-fluid"/>
        </div>
      </div>
    </div>
</template>
  
  <script>
  export default {
    name: "BrandSlide",
    data() {
        return {
        brands: [
            { name: "Brand 1", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 2", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 3", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 4", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 5", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 6", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 7", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 8", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 9", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 10", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 11", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 12", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 13", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 14", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 15", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 16", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 17", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
            { name: "Brand 18", logo: "https://image.freepik.com/free-vector/3d-box-logo_1103-876.jpg" },
        ],
        currentIndex: 0,
        currentOffset: 0,
        };
    },
    computed: {
        itemWidth() {
        // Sesuaikan dengan lebar item (misalnya, 100px untuk logo)
        return 100;
        },
    },
    methods: {
        nextSlide() {
        if (this.currentIndex < this.brands.length - 1) {
            this.currentIndex++;
        } else {
            this.currentIndex = 0;
        }
        this.currentOffset = this.currentIndex * this.itemWidth;
        },
    },
    mounted() {
        setInterval(this.nextSlide, 5000); // Ganti slide setiap 5 detik
    },
  };
  </script>
  
  <style scoped>
  .brand-slider {
  width: 100%;
  max-width: 1000px; /* Sesuaikan sesuai kebutuhan */
  margin: auto;
}

.brand-track {
  display: flex;
  transition: transform 1s ease;
}

.brand-item {
  width: 100px; /* Lebar item/logo */
  flex-shrink: 0;
  margin-right: 20px; /* Jarak antar logo */
}
  </style>
  