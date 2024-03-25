<template>
  <div id="projects-card">
    <div class="text-content">
        <h3>Meus Projetos</h3>
        <p>Alguns projetos feitos por mim</p>
    </div>
    <div class="cards-content">
        <CardProjects class="CardProjects">
            <template #image>
                <img src="@/assets/asppe-project.png">
            </template>
            <h2>ASPPE VUE</h2>
            <p>
                Projeto feito totalmente em Vue para a Associação dos Pescadores onde os participantes poderão ver os resultados das etapas. Para mostrar os resultados eu fiz uma integração com o Google Sheets e isso facilita, pois quando eu inserir os resultados das etapas será alterado automaticamente no site.
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
               A API do AL Caronas surgiu através da ideia de criar um sistema onde pessoas pudessem se cadastrar, fornecer os dados necessários e a partir daí buscar por caronas que fossem para o mesmo destino que, fazendo com que economizasse uma certa quantia, tanto ela como o motorista. O projeto foi feito em C#/.NET, Entity Framework e MySQL.
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
               O DontoSync é mais um ideia pessoal minha onde seria basicamente um sistema que possibilitaria o cadastro de pacientes e todo o controle por parte dos dentista ajudando os mesmos a organizarem mais o seus atendimentos. A partir dessa ideia o primeiro passo foi criar um API que possibilitasse o cadastro desses pacientes. O projeto foi feito em C#/.NET, Entity Framework e MySQL.
            </p>
            <a href="https://github.com/Ol1veirx/DontoSync-API" target="_blank">🔗Link Do Repositório</a>
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
}

.text-content{
    margin-bottom: 55px
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
