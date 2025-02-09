<script setup>
import { RouterLink, RouterView } from 'vue-router'
import NavComponent from './components/navigation/NavComponent.vue'
</script>

<template class="app-view grid">
  <header>
    <NavComponent/>
  </header>

  <RouterView />
</template>
<style lang="scss">
// @import '@/assets/scss/global.scss'
    
</style>
