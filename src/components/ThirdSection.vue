<template>
  <div id="projects-card">
    <div class="text-content">
        <h3>Meus Projetos</h3>
        <p>Alguns projetos feitos por mim</p>
    </div>
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

@media (max-width: 768px){
    .CardProjects{
        margin: 0 auto
    }
}
</style>
