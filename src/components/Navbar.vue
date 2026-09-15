<template>
  <header class="navbar" :class="{ scrolled: isScrolled }">
    <nav class="navbar-container">
      <div class="navbar-inner">
        <RouterLink to="/" class="navbar-logo" aria-label="JB Agency - Ir al inicio">
          <!-- <img src="/images/Logo.png" alt="JB Agency" /> -->
        </RouterLink>
      </div>
    </nav>
  </header>
</template>

<script setup lang="ts">
import { RouterLink } from 'vue-router'
import { onMounted, onUnmounted, ref } from 'vue'

const isScrolled = ref(false)

const handleScroll = () => {
  isScrolled.value = window.scrollY > 10
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll, { passive: true })
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})

defineOptions({ name: 'PikiitosNavbar' })
</script>

<style>
.navbar {
  position: sticky;
  top: 0;
  z-index: 50;
  background-color: rgba(250, 248, 245, 0.95);
  backdrop-filter: blur(24px);
  -webkit-backdrop-filter: blur(24px);
  transition: all 0.3s ease;
}

.navbar.scrolled {
  box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
}

.navbar-container {
  max-width: 80rem;
  margin: 0 auto;
  padding: 0 1rem;
}

@media (min-width: 640px) {
  .navbar-container {
    padding: 0 1.5rem;
  }
}

@media (min-width: 1024px) {
  .navbar-container {
    padding: 1rem 2rem;
  }
}

.navbar-inner {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 4rem;
  gap: 1rem;
}

@media (min-width: 1024px) {
  .navbar-inner {
    height: 4rem;
  }
}

.navbar-logo {
  flex-shrink: 0;
  display: flex;
  align-items: center;
}

.navbar-logo img {
  height: 4rem;
  width: auto;
  object-fit: contain;
}

@media (min-width: 1024px) {
  .navbar-logo img {
    height: 5rem;
  }
}
</style>
