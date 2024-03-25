<template>
    <div class="main-content">
        <div class="content-about">
            <h2>
                Sobre Mim
            </h2>
            <p>
                Olá! Sou Liedson Danubio Oliveira Leite, um entusiasta incansável da tecnologia e estudante de Sistemas da Informação na renomada UFAL, onde atualmente estou no 4º período. Desde que entrei nesse emocionante mundo da programação há pouco mais de dois anos, tenho sido cativado pela beleza e pela complexidade desse universo digital em constante evolução.
            </p>
            <p>
                Ao longo dessa jornada, desenvolvi uma sólida compreensão em diversas stacks, explorando tanto o mundo do front-end quanto do back-end. No entanto, recentemente, direcionei minha paixão e curiosidade para a fascinante esfera do desenvolvimento back-end, particularmente com C#/.NET. Através desse enfoque, tenho me desafiado a alcançar novos patamares de excelência e a aprimorar minhas habilidades em um dos ecossistemas tecnológicos mais robustos do mercado.
            </p>
            <p>
                Para mim, a aprendizagem é mais do que uma simples jornada acadêmica; é uma paixão ardente e uma missão pessoal. Tenho uma fome insaciável por conhecimento e uma habilidade natural para absorver novas informações rapidamente. Acredito firmemente que o aprendizado contínuo é a chave para o crescimento pessoal e profissional, e estou sempre em busca de novas oportunidades para expandir meus horizontes e desafiar minhas próprias limitações.
            </p>
            <p>
                Movido por uma determinação inabalável e uma visão clara do que desejo alcançar, estou comprometido em seguir adiante com coragem e confiança. Acredito firmemente que o futuro pertence àqueles que ousam sonhar grande, trabalhar incansavelmente e nunca se contentar com menos do que aquilo em que acreditam.
            </p>
            <p>
                Estou ansioso para as emocionantes aventuras que o futuro reserva e para as oportunidades emocionantes que aguardam pela frente. Com dedicação, paixão e uma mente aberta para novos desafios, estou pronto para enfrentar o que quer que o destino me reserve e para transformar meus sonhos em realidade.
            </p>
            <h4>Formação</h4>
            <p>
                ✅ Ensino Médio Técnico em Açúcar e Álcool - IFAL (2018-2022)
            </p>
            <p>
                ✅ Bacharel em Sistemas da Informação - UFAL (4° Período)
            </p>
        </div>
        <div class="img-about">
            <img src="@/assets/ol1veirx.png">
        </div>
    </div>
</template>

<script>

</script>

<style scoped>
.main-content{
    display: flex;
    align-items: center;
    justify-content: space-around;

    padding: 20px;
}

.content-about{
    width: 50%;
}

.content-about h2, h4 {
    margin-bottom: 20px;
}

.content-about p{
    text-align: justify;
}

.img-about img{
    width: 150px;
}

@media (max-width: 768px){
    .main-content{
        flex-direction: column;
    }

    .content-about{
        width: 90%;
    }   
}
</style>