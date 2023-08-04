<template>
    <div class="home">
      <div ref="lottieContainer"></div>
    </div>
  </template>
    
  <script setup>
  import { onMounted, ref } from "vue";
  import Lottie from "lottie-web";
  import animationData from "@/assets/animation_lkw5yegy.json";
  
  const lottieContainer = ref(null);
  const anim = ref(null);
  
  onMounted(() => {
    anim.value = Lottie.loadAnimation({
      container: lottieContainer.value,
      renderer: "svg",
      loop: true,
      autoplay: true,
      animationData: animationData,
    });
  });
  </script>
    
  <style scoped>
  .home {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
  </style>