<template>
  <div class="maintenance-wrapper">
    <div class="maintenance-container">
      <!-- Lado izquierdo -->
      <div class="maintenance-left">
        <div class="left-text-block">
          <img src="/images/Saludo.png" alt="Saludo" class="saludo-hand" />
          <p class="left-line-1">Estamos dedicando</p>
          <p class="left-line-italic">tiempo,</p>
          <p class="left-line-italic">intención y</p>
          <p class="left-line-italic">cuidado</p>
          <p class="left-line-normal">a la renovación de este</p>
          <p class="left-line-normal">sitio, nuestro lugar de</p>
          <p class="left-line-normal">contacto.</p>
        </div>
        <img src="/images/Conos.png" alt="Construcción" class="conos-image" />
      </div>

      <!-- Línea divisoria -->
      <div class="maintenance-divider"></div>

      <!-- Lado derecho -->
      <div class="maintenance-right">
        <div class="ok-block">
          <img src="/images/Correo.png" alt="OK" class="ok-hand" />
          <div class="ok-content">
            <span class="ok-line-1">Por ahora, hablemos en:</span>
            <a href="mailto:director@jbagencyco.com" class="ok-line-2">director@jbagencyco.com</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
defineOptions({ name: 'Maintenance' })
</script>

<style scoped>
.maintenance-wrapper {
  min-height: 50vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #FAF8F5;
  padding: 2rem 1rem 0;
  margin-bottom: 0;
}

.maintenance-container {
  max-width: 64rem;
  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  margin-left: 5%;
}

.maintenance-left {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding-right: 3rem;
  padding-left: 2rem;
}

.left-text-block {
  position: relative;
  padding-left: 0.5rem;
}

.saludo-hand {
  position: absolute;
  top: -30px;
  left: -70px;
  height: 80px;
  width: auto;
  object-fit: contain;
}

.left-line-1 {
  font-family: 'OptimaMedium', serif;
  font-size: 1.85rem;
  font-weight: 300;
  color: #1a1a1a;
  line-height: 1;
  letter-spacing: 0.05em;
  margin: 0 0 0.1rem 0;
}

.left-line-italic {
  font-family: 'OptimaMedium', serif;
  font-size: 1.85rem;
  font-weight: 500;
  color: #8F8A5B;
  line-height: 1.1;
  letter-spacing: 0.05em;
  margin: 0;
}

.left-line-normal {
  font-family: 'OptimaMedium', serif;
  font-size: 1.85rem;
  font-weight: 300;
  color: #1a1a1a;
  line-height: 1.1;
  letter-spacing: 0.05em;
  margin: 0;
}

.conos-image {
  width: 200px;
  height: auto;
  object-fit: contain;
  margin-top: -3.0rem;
  margin-left: 8.5rem;
}

.maintenance-right {
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  padding-left: 3rem;
}

.ok-block {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 1.25rem;
}

.ok-hand {
  height: 100px;
  width: auto;
  object-fit: contain;
  transform: rotate(35deg);
  flex-shrink: 0;
  margin-right: -35px;
  position: relative;
  z-index: 10;
  margin-bottom: 60px;
}

.ok-content {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 4px;
}

.ok-line-1 {
  font-family: 'OptimaMedium', serif;
  font-size: 25px;
  font-weight: 300;
  color: #3a3a3a;
  line-height: .8;
}

.ok-line-2 {
  font-family: 'OptimaItalic', serif;
  font-size: 22px;
  font-weight: 400;
  color: #3a3a3a;
  text-decoration: none;
  line-height: 1.3;
  transition: color 0.2s ease;

}

.ok-line-2:hover {
  color: #C49A6C;
}

.maintenance-divider {
  width: 3px;
  height: 20rem;
  background-color: rgba(37, 33, 27, 0.658);
  flex-shrink: 0;
  margin-top: -4rem;
  margin-right: 5rem;
}

@media (max-width: 768px) {
  .maintenance-container {
    flex-direction: column;
    gap: 2rem;
  }

  .maintenance-divider {
    width: 100%;
    height: 1px;
    background-color: rgba(196, 154, 108, 0.3);
  }

  .maintenance-left,
  .maintenance-right {
    align-items: center;
    text-align: center;
  }

  .ok-block {
    flex-direction: column;
    text-align: center;
  }

  .ok-content {
    align-items: center;
  }
}
</style>
