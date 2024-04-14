<template >
  <section class="main-content">
    <div class="text-content">
      <span>Hello <div class="hand">👋🏽</div>, I'm</span>
      <h1>Liedson Danubio</h1>
      <h2>Software <span class="engineer-name">Engineer</span></h2>
      <div class="btn-sayHello">
        <a href="mailto:liedsonleite3@hotmail.com">Say hello</a>
      </div>
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
  margin-top: 150px;
}

.text-content{
  display: flex;
  align-items: first baseline;
  justify-content: center;
  flex-direction: column;
}

.text-content span {
  font-size: 30px;
  text-align: left;
  font-weight: bold;
}

.text-content h1 {
  font-size: 80px;
  font-weight: bold;
  color: #2c3e50;
}

.text-content h2{
  font-size: 60px;
  font-weight: bold;
  color: #2c3e50;
  text-shadow: 1px 2px 8px rgba(0, 0, 0, 0.24);
}

.text-content h2 span{
  font-size: 60px;
  font-weight: bold;
  color: #c97309;
  text-shadow: 1px 2px 8px rgba(0, 0, 0, 0.24);
}

.btn-sayHello {
  font-size: 20px;
  background-color: #c97309;
  padding: 5px;
  border-radius: 8px;
  width: 150px;
  color: #2c3e50;
  box-shadow: 1px 2px 8px rgba(0, 0, 0, 0.438);
  cursor: pointer;
  transition: transform 0.3s ease;
}

.btn-sayHello a{
  text-decoration: none;
  color: #2c3e50;
}

.btn-sayHello:hover {
   transform: scale(1.05);
}

.img-content img{
  width: 450px;
  border-radius: 50%;
  box-shadow: 1px 2px 8px rgba(0, 0, 0, 0.418);
  filter: grayscale(100%); 
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

@media (max-width: 768px){
  .main-content{
    text-align: left;
    padding: 10px;
  }
  .btn-sayHello{
    text-align: center;
  }
  .img-content{
    display: none;
  }
}
</style>