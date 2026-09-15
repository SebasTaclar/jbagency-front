<template>
  <footer class="footer">
    <div class="footer-content">
      <!-- Logo -->
      <img src="/images/Logo.png" alt="JB Agency Logo" class="footer-logo" />
    </div>

    <div class="footer-bottom">
      <p class="footer-tagline">Estrategia y creatividad con propósito</p>
      <p class="footer-copyright">&copy; {{ new Date().getFullYear() }} JB Agency. Todos los derechos reservados.</p>
    </div>
  </footer>
</template>

<script setup lang="ts">
defineOptions({ name: 'FooterSection' })
</script>

<style scoped>
.footer {
  background-color: #FAF8F5;
  padding: 0rem 1rem;
}

.footer-content {
  max-width: 80rem;
  margin: 0 auto;
  display: flex;
  justify-content: center;
}

.footer-logo {
  height: 4.3rem;
  width: auto;
  object-fit: contain;
}

.footer-bottom {
  max-width: 80rem;
  margin: 0.75rem auto 0;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
}

.footer-tagline {
  font-family: 'OptimaMedium', serif;
  font-size: 11px;
  color: rgba(26, 26, 26, 0.4);
  margin: 0;
}

.footer-copyright {
  position: absolute;
  right: 0;
  font-family: 'OptimaMedium', serif;
  font-size: 11px;
  color: rgba(26, 26, 26, 0.4);
  margin: 0;
}

@media (max-width: 768px) {
  .footer-bottom {
    flex-direction: column;
    align-items: center;
    gap: 0.25rem;
  }

  .footer-copyright {
    position: static;
  }
}
</style>
