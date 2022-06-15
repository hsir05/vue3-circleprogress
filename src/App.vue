<template>
  <div class="">
    <CircleProgress :progress="progress" color="#fdd835"  />
  </div>
</template>
<script setup>
import { ref } from "vue"
import CircleProgress from "./components/circleProgress.vue";

const progress = ref(50)
setInterval(() => {
    progress.value = Math.floor(Math.random()*100+1)
}, 1000);
</script>

