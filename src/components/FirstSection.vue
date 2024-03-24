<template >
  <section class="main-content">
    <div class="text-content">
      <h2>Olá <div class="hand">👋🏽</div>,<br>Eu sou<br><span>Liedson Danubio</span><br> Sou Dev Back-End</h2>
    </div>

    <div class="img-content">
        <img src="@/assets/MyImg.png" alt="Imagem" class="img-fluid" />
      </div>
  </section>
</template>

<script>
export default {
  name: 'HomeSection',
}
</script>

<style scoped>
.main-content{
  display: flex;
  align-items: center;
  justify-content: space-around;
  margin-top: 30px;
}

.text-content h2{
  font-size: 60px;
  text-align: left;
  color: #404e03;
  text-shadow: 1px 2px 8px rgba(0, 0, 0, 0.24);
}

.hand {
  display: inline-block;
  animation: waveAnimation 2s infinite ease-in-out alternate;
}

@keyframes waveAnimation {
  0% {
    transform: rotate(0deg);
  }
  20% {
    transform: rotate(20deg);
  }
  40% {
    transform: rotate(0deg);
  }
  60% {
    transform: rotate(20deg);
  }
  80% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(0deg);
  }
}

.text-content h2 span{
  background: linear-gradient(to right, #1b2201, rgb(198, 241, 5)); 
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
}

.img-content img{
  width: 450px;
  border-radius: 50%;
  box-shadow: 1px 2px 8px rgba(0, 0, 0, 0.418);
  filter: grayscale(100%); 
}

@media (max-width: 768px){
  .img-content{
    display: none;
  }
}
</style>