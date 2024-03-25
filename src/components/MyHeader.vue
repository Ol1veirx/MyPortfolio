<template>
  <header class="navbar navbar-expand-lg navbar-light bg-white">
    <div class="container d-flex justify-content-between align-items-center header-container">
      <!-- Logo no lado esquerdo -->
      <router-link to="/" class="navbar-brand">
        <img src="@/assets/logo-header.png" alt="Logo" class="mr-5" />
      </router-link>

      <button class="navbar-toggler" type="button" @click="toggleMenu" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Links do menu -->
      <div class="collapse navbar-collapse" :class="{ 'show': isMenuOpen }" id="navbarNav">
        <button v-if="isMenuOpen" class="close-button" @click="toggleMenu" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
        <ul class="navbar-nav">
          <li class="nav-item">
            <router-link to="/" class="nav-link">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/about" class="nav-link">Sobre</router-link>
          </li>
        </ul>
      </div>

      <div class="d-lg-flex flex-row align-items-center link-icons">
        <a href="https://github.com/Ol1veirx" target="_blank" class="nav-link"><img src="@/assets/github.svg" alt="GitHub" class="contacts-icon" /></a>
        <a href="https://www.linkedin.com/in/liedson-d-o-leite/" target="_blank" class="nav-link"><img src="@/assets/linkedin.svg" alt="LinkedIn" class="contacts-icon" /></a>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'MyHeader',
  data() {
    return {
      isMenuOpen: false
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    }
  }
}
</script>


<style scoped>
.header-container::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 2px;
  background: linear-gradient(to right, #1b2201, rgb(198, 241, 5));
}

.navbar-brand img {
  width: 70px;
}

.contacts-icon {
  width: 35px;
  margin: 8px;
}

.nav-link {
  color: rgb(77, 77, 77);
  font-weight: 500;
}

.nav-link img {
  width: 55px;
}

@media (max-width: 768px) {
  .navbar-collapse {
    position: fixed;
    top: 0;
    left: 0;
    height: 100vh;
    width: 100%;
    background-color: rgba(255, 255, 255, 0.9);
    z-index: 1000;
    overflow-y: auto;
    transform: translateX(-100%);
    transition: transform 0.3s ease;
  }

  .link-icons{
    display: none
  }

  .navbar-collapse.show {
    transform: translateX(0%);
  }

  .navbar-nav {
    width: 100%;
    text-align: center;
  }

  .navbar-nav .nav-item {
    margin: 15px 0;
  }

  .close-button {
    position: absolute;
    top: 0.5rem;
    right: 0.5rem;
    font-size: 1.5rem;
    background-color: transparent;
    border: none;
    cursor: pointer;
  }
}
</style>
