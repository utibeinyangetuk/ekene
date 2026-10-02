<template>
  <div class="carousel" @mouseenter="stopAutoplay" @mouseleave="startAutoplay">
    <Transition name="fade" mode="out-in">
      <img :key="currentIndex" :src="images[currentIndex]" class="slide-image" alt="Carousel Image" />
    </Transition>
    <!-- Pagination -->
    <div v-if="pagination" class="pagination">
      <span v-for="(_, index) in images" :key="index" :class="{ active: currentIndex === index }"
        @click="currentIndex = index">
      </span>
    </div>
  </div>
</template>

<script setup>
  import { onMounted, onUnmounted, ref } from "vue";

  const props = defineProps({
    images: {
      type: Array,
      required: true,
    },
    interval: {
      type: Number,
      default: 5000,
    },
    pagination: {
      type: Boolean,
      default: true,
    },
    autoplay: {
      type: Boolean,
      default: true,
    },
  });

  const currentIndex = ref(0);

  let timer = null;

  const nextSlide = () => {
    currentIndex.value =
      (currentIndex.value + 1) % props.images.length;
  };

  const prevSlide = () => {
    currentIndex.value =
      (currentIndex.value - 1 + props.images.length) %
      props.images.length;
  };

  const startAutoplay = () => {
    if (!props.autoplay) return;

    stopAutoplay();

    timer = setInterval(() => {
      nextSlide();
    }, props.interval);
  };

  const stopAutoplay = () => {
    if (timer) clearInterval(timer);
  };

  onMounted(startAutoplay);
  onUnmounted(stopAutoplay);
</script>

<style scoped>
  .carousel {
    width: 100%;
    /* aspect-ratio: 16 / 9; */
    height: 700px;
    overflow: hidden;
  }

  .slide-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
    border-radius: var(--border-radius);
    border: var(--border);
  }

  /* Fade Animation */
  .fade-enter-active,
  .fade-leave-active {
    transition: opacity 1s ease;
  }

  .fade-enter-from,
  .fade-leave-to {
    opacity: 0;
  }

  /* Pagination */
  .pagination {
    position: absolute;
    bottom: 10px;
    width: 50%;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    justify-content: space-evenly;
    z-index: 3;
  }

  .pagination span {
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background: rgba(255, 255, 255, 0.5);
    cursor: pointer;
    border: 1px solid;
  }

  .pagination span.active {
    background: var(--prybackground);
  }

  @media (max-width: 768px) {
    .carousel {
      aspect-ratio: 16 / 9;
      height: 100%;
    }
  }

  @media (max-width: 600px) {
    .carousel {
      aspect-ratio: 16 / 9;
      height: 100%;
    }
  }
</style>