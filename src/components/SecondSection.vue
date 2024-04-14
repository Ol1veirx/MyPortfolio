<template>
    <section class="second-section">
        <div class="text-content">
            <h3>My Technologies</h3>
            <span>Technologies I work with</span>
        </div>

        <div class="icon-techs">
            <img src="@/assets/VS.svg" class="floating-img"/>
            <img src="@/assets/vsCode.svg" class="floating-img"/>
            <img src="@/assets/csharp.svg" class="floating-img"/>
            <img src="@/assets/.net.png" style="width: 65px;" class="floating-img"/>
            <img src="@/assets/sql.png" class="floating-img"/>
            <img src="@/assets/mongo.svg" class="floating-img"/>
            <br>
            <img src="@/assets/html.svg" class="floating-img"/>
            <img src="@/assets/css.svg" class="floating-img"/>
            <img src="@/assets/JS.svg" class="floating-img"/>
            <img src="@/assets/vue.svg" class="floating-img"/>
            <img src="@/assets/docker.svg" class="floating-img"/>
            <img src="@/assets/insomnia.png" style="width: 65px;" class="floating-img"/>
        </div>
    </section>
</template>

<script>
export default {
    name: 'SecondSection'
}
</script>

<style scoped>
.second-section{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 35px;
    margin-top:400px;
    background-color: rgb(216, 215, 215);
    height: 900px;
    box-shadow: 1px 2px 8px rgba(0, 0, 0, 0.432);
}

.text-content h3{
    font-weight: bold;
    font-size: 50px;
}

.floating-img {
  animation: floatAnimation 2s infinite ease-in-out alternate;
}

@keyframes floatAnimation {
  0% {
    transform: translateY(0);
  }
  100% {
    transform: translateY(-10px);
  }
}

.icon-techs img{
    margin: 25px 65px
}

@media (max-width: 768px){
    .text-content h3{
        font-size: 31px;
    }

     .text-content span{
        font-size: 18px
     }

     .icon-techs img{
        width: 75px;
     }
}
</style>