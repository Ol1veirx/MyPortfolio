<template>
    <div class="main-content">
        <div class="content-about">
            <h2>
                About Me
            </h2>
            <p>
                Hello! I'm Liedson Danubio Oliveira Leite, a tireless technology enthusiast and Information Systems student at the renowned UFAL, where I'm currently in the 4th period. Since entering this exciting world of programming just over two years ago, I have been captivated by the beauty and complexity of this constantly evolving digital universe.
            </p>
            <p>
                Along this journey, I developed a solid understanding of various stacks, exploring both the front-end and back-end worlds. However, recently I have turned my passion and curiosity into the fascinating sphere of back-end development, particularly with C#/.NET. Through this approach, I have challenged myself to reach new levels of excellence and improve my skills in one of the most robust technological ecosystems on the market.
            </p>
            <p>
                For me, learning is more than just an academic journey; it is a burning passion and a personal mission. I have an insatiable hunger for knowledge and a natural ability to absorb new information quickly. I firmly believe that continuous learning is the key to personal and professional growth, and I am always looking for new opportunities to expand my horizons and challenge my own limitations.
            </p>
            <p>
                Driven by unwavering determination and a clear vision of what I want to achieve, I am committed to moving forward with courage and confidence. I firmly believe that the future belongs to those who dare to dream big, work tirelessly and never settle for less than what they believe in.
            </p>
            <p>
                I look forward to the exciting adventures the future holds and the exciting opportunities that lie ahead. With dedication, passion and an open mind to new challenges, I am ready to face whatever fate has in store for me and to turn my dreams into reality.
            </p>
            <h4>Education</h4>
            <p>
                ✅ Technical High School in Sugar and Alcohol - IFAL (2018-2022)
            </p>
            <p>
                ✅ Bachelor of Information Systems - UFAL (4th Period)
            </p>
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