<template>
  <div class="link-box">
    <div class="img-box">
      <slot name="image"></slot>
    </div>
    <div class="details-box">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProjectCard',
}
</script>

<style scoped>
.link-box {
  display: flex;
  flex-direction: column;
  cursor: pointer;
  border: 1px solid #ccc;
  border-radius: 8px;
  overflow: hidden;
  transition: box-shadow 0.3s ease;

  width: 300px;
}

.link-box:hover {
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.img-box {
  width: 100%;
  height: 200px;
  overflow: hidden;
  border-bottom: 1px solid rgba(0, 0, 0, 0.473);
}

.img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.details-box {
  padding: 20px;
}

/* Estilos opcionais para tornar o componente mais responsivo */
@media (max-width: 768px) {
  .img-box {
    height: 150px;
  }
}
</style>