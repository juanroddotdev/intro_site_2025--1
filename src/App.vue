<script setup>
import { RouterLink, RouterView } from 'vue-router'
import NavComponent from './components/navigation/NavComponent.vue'
import { useTheme } from './composables/useTheme'
import { provide } from 'vue'

const theme = useTheme()
provide('theme', theme)
const { currentTheme } = theme;
</script>

<template>
  <div class="theme" :class="currentTheme">
    <header>
      <NavComponent/>
    </header>

    <RouterView />
  </div>
</template>
<style lang="scss">
// @import '@/assets/scss/global.scss'

    
</style>
