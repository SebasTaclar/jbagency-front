<template>
  <div class="min-h-screen bg-[#FAF8F5]">
    <!-- <Navbar /> -->

    <Maintenance />

    <!-- <Footer_ /> -->
  </div>
</template>

<script setup lang="ts">
import Navbar from '@/components/Navbar.vue'
import Footer_ from '@/components/Footer_.vue'
import Maintenance from '@/views/Maintenance.vue'

defineOptions({ name: 'App' })
</script>
