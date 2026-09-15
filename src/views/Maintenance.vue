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

    <div class="maintenance-footer">
      <img src="/images/Logo.png" alt="JB Agency" class="maintenance-logo" />
      <p class="maintenance-copyright">Estrategia y creatividad con propósito</p>
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
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: #FAF8F5;
  padding-top: 5rem;
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
  padding-right: 4rem;
  padding-left: 1rem;
}

.left-text-block {
  position: relative;
  padding-left: 0.5rem;
}

.saludo-hand {
  position: absolute;
  top: -40px;
  left: -70px;
  height: 80px;
  width: auto;
  object-fit: contain;
}

.left-line-1 {
 font-size: 36px;
  font-family: 'OptimaMedium', serif;
  font-weight: 300;
  font-style: normal;
  color: #635F5C;
  font-display: swap;
}

.left-line-italic {
  font-family: 'OptimaMedium', serif;
  font-size: 34px;
  font-weight: 600;
  color: #999b6e;
  line-height: 1.3;
  margin: 0;
  font-style: italic;
}

.left-line-normal {
  font-family: 'OptimaMedium', serif;
  font-size: 36px;
  font-weight: 300;
  color: #635F5C;
  line-height: 1.2;
  margin: 0;
}

.conos-image {
  width: 190px;
  height: auto;
  object-fit: contain;
  margin-top: -3.5rem;
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
  font-family: 'OptimaRegular', serif;
  font-size: 28px;
  font-weight: 300;
  color: #635F5C;
  line-height: 1.2;
}

.ok-line-2 {
  font-family: 'OptimaRegular', serif;
  font-size: 24px;
  font-weight: 400;
  color: #635F5C;
  line-height: .8;
  font-style: italic;
}

.ok-line-2:hover {
  color: #C49A6C;
}

.maintenance-divider {
  width: 3px;
  height: 26rem;
  background-color: rgba(37, 33, 27, 0.658);
  flex-shrink: 0;
  margin-top: -3rem;
  margin-right: 5rem;
}

.maintenance-footer {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.maintenance-logo {
  height: 4rem;
  width: auto;
  object-fit: contain;
}

.maintenance-copyright {
  font-family: 'Optimamedium', serif;
  font-size: 10px;
  color: #635F5C;
  font-weight: 600;
}

@media (max-width: 768px) {
  .maintenance-wrapper {
    padding: 4rem 1rem 0;
  }

  .maintenance-container {
    flex-direction: column;
    gap: 0;
    margin-left: 0;
  }

  .maintenance-left {
    padding-left: 0;
    padding-right: 0;
    align-items: flex-start;
    margin-bottom: 1rem;
  }

  .saludo-hand {
    top: -40px;
    left: -40px;
    height: 55px;
  }

  .left-line-1,
  .left-line-italic,
  .left-line-normal {
    font-size: 18px;
  }

  .conos-image {
    margin-left: 90px;
    margin-right: auto;
    margin-top: -1rem;
    width: 120px;
  }

  .maintenance-divider {
    width: auto;
    height: 2px;
    background-color: rgba(37, 33, 27, 0.658);
    margin: 1rem 3rem;
    align-self: stretch;
  }

  .maintenance-right {
    padding-left: 0;
    align-items: flex-start;
    justify-content: flex-start;
    margin-top: 2rem;
    margin-bottom: 2rem;
  }

  .ok-block {
    flex-direction: row;
    align-items: center;
    gap: 0.25rem;
    padding-right: 2.65rem;
    padding-top: 2rem;
  }

  .ok-hand {
    height: 55px;
    transform: rotate(35deg);
    margin-right: -17px;
    margin-bottom: 40px;
  }

  .maintenance-copyright {
    font-size: 9px;
  }

  .ok-content {
    align-items: flex-start;
  }

  .ok-line-1 {
    font-size: 16px;
  }

  .ok-line-2 {
    font-size: 14px;
  }

  .maintenance-logo {
    height: 2.5rem;
  }
}
</style>
