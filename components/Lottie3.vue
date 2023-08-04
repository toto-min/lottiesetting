<template>
    <div>
        <client-only>
            <Vue3Lottie :animationData="playJSON" :height="200" :width="200" />
        </client-only>
    </div>
</template>
<script setup>
import playJSON from '@/assets/animation_lkw5yegy.json'
</script>