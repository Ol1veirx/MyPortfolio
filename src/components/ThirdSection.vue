<template>
  <div id="projects-card">
    <div class="text-content">
        <h3>My <span>Projects</span></h3>
        <p>Portfólio</p>
    </div>
    <div class="cards-content">
        <CardProjects class="CardProjects">
            <template #image>
                <img src="@/assets/asppe-project.png">
            </template>
            <h2>ASPPE VUE</h2>
            <p>
                Project made entirely in Vue for the Fishermen's Association where participants will be able to see the results of the stages. To show the results I integrated with Google Sheets and this makes it easier, because when I insert the results of the steps it will automatically change on the website.
            </p>
            <a href="https://asppepenedo.vercel.app" target="_blank">🔗Link Do Site</a>
            <a href="https://github.com/Ol1veirx/ASPPE-VUE" target="_blank">🔗Link Do Repositório</a>
        </CardProjects>

         <CardProjects class="CardProjects">
            <template #image>
                <img class="img-project2" src="@/assets/travel.jpg">
            </template>
            <h2>AL Caronas - API</h2>
            <p>
               The AL Caronas API came about through the idea of creating a system where people could register, provide the necessary data and from there search for rides that went to the same destination, saving a certain amount, both themselves and the driver. The project was created in C#/.NET, Entity Framework and MySQL.
            </p>
            <a href="https://github.com/Ol1veirx/AL_CARONAS-API" target="_blank">🔗Link Do Repositório</a>
        </CardProjects>

        <CardProjects class="CardProjects">
            <template #image>
                <img class="img-project2" src="@/assets/odonto.jpg">
                <img  src="@/assets/asppe-project.png">
            </template>
            <h2>DontoSync - API</h2>
            <p>
               DontoSync is another personal idea of mine where it would basically be a system that would enable patient registration and full control by dentists, helping them to better organize their care. Based on this idea, the first step was to create an API that would allow these patients to register. The project was created in C#/.NET, Entity Framework and MySQL.
            </p>
            <a href="https://github.com/Ol1veirx/DontoSync-API" target="_blank">🔗Link Do Repositório</a>
        </CardProjects>

        <CardProjects class="CardProjects">
            <template #image>
                <img class="img-project2" src="@/assets/FishPro.png">
                <img  src="@/assets/asppe-project.png">
            </template>
            <h2>FishPro - API</h2>
            <p>
               FishPro is a web application designed to allow users to create, manage and track sports tournaments. This document describes the overall architecture of the system, including its data structure, use cases, and user interaction flows.
            </p>
            <a href="https://github.com/Ol1veirx/FishPro---API" target="_blank">🔗Link Do Repositório</a>
        </CardProjects>
    </div>
  </div>
</template>

<script>
import CardProjects from '@/components/CardProjects.vue';

export default {
  name: 'ThirdSection',
  components: {
    CardProjects
  },
}
</script>

<style scoped>
#projects-card{
    margin-top: 50px;
    padding: 55px;
    height: 900px;
}

.text-content{
    margin-bottom: 55px
}

.text-content h3 {
    font-weight: bold;
    font-size: 50px;
}

.text-content span {
    color: #c97309;
}

a{
    text-decoration: none;
    font-size: 14px;
    color: rgb(66, 94, 2)
}

.cards-content{
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.img-project2{
    width: 400px;
}

@media (max-width: 768px){
    .CardProjects{
        margin: 0 auto;
    }

    #projects-card{
        margin-bottom: 40px;
        padding: 0;
    }

    .cards-content{
        flex-direction: column;
        gap: 35px;
}
}
</style>
