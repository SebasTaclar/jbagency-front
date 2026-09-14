<template>
  <main class="home-main">
    <div class="min-h-screen flex flex-col items-center justify-center px-6 py-16 md:py-24">
      <div class="max-w-2xl w-full flex flex-col items-start">
        <span class="text-5xl md:text-6xl mb-2 animate-wiggle">👋</span>

        <h1 class="text-3xl md:text-[2.6rem] leading-snug font-normal text-jbagency-charcoal mt-4">
          Estamos dedicando
          <span class="italic text-jbagency-olive">tiempo,</span>
          <span class="italic text-jbagency-olive">intención y</span>
          <span class="italic text-jbagency-olive">cuidado</span>
          a la renovación de este sitio, nuestro lugar de contacto.
        </h1>
      </div>

      <div class="mt-12 md:mt-16">
        <span class="text-6xl md:text-8xl">🚧</span>
      </div>

      <div class="w-full max-w-md my-14 md:my-20 border-t border-gray-300"></div>

      <div class="max-w-2xl w-full flex flex-col items-start">
        <div class="flex items-center gap-4">
          <span class="text-5xl md:text-6xl">👌</span>
          <p class="text-xl md:text-2xl text-jbagency-charcoal">
            Por ahora, hablemos en:<br />
            <a href="mailto:director@jbagencyco.com" class="italic text-jbagency-olive hover:underline">
              director@jbagencyco.com
            </a>
          </p>
        </div>
      </div>

      <div class="mt-16 md:mt-24 flex flex-col items-center gap-3">
        <div class="flex items-center gap-2">
          <svg class="w-12 h-12 md:w-14 md:h-14" viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M50 5C25.2 5 5 25.2 5 50s20.2 45 45 45 45-20.2 45-45S74.8 5 50 5z" fill="#000" />
            <path d="M38 30h8l8 18-8 18h-8l8-18L38 30z" fill="#fff" />
            <path d="M52 30h8l8 18-8 18h-8l8-18-8-18z" fill="#fff" />
          </svg>
        </div>
        <span class="text-sm md:text-base tracking-[0.3em] text-jbagency-olive font-medium uppercase">
          JB Agency
        </span>
        <p class="text-sm md:text-base text-jbagency-gray">
          Estrategia y creatividad con propósito
        </p>
      </div>
    </div>
  </main>
</template>

<script setup lang="ts">
defineOptions({ name: 'HomeView' })
</script>

<style scoped>
.home-main {
  background: #F0EDE8;
  min-height: 100vh;
}
</style>
