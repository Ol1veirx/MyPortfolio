<template>
    <div id="aboutmeSection">
        <div class="img-content">
            <img src="@/assets/img-about.jpg">
        </div>
        <div class="text-content">
            <h3>About <span>Me</span></h3>
            <p>Passionate about programming</p>
            <ul>
                <li>Information Systems Student (4th period)</li>
                <li>1 year experience</li>
                <li>B1 intermediate level</li>
            </ul>
            <router-link to="/about" class="about-link">
                More About Me
            </router-link>
            <div class="img-links">
                <a href="https://github.com/Ol1veirx" target="_blank" class="nav-link"><img src="@/assets/github.svg" alt="GitHub" class="contacts-icon" /></a>
                <a href="https://www.linkedin.com/in/liedson-d-o-leite/" target="_blank" class="nav-link"><img src="@/assets/linkedin.svg" alt="LinkedIn" class="contacts-icon" /></a>
            </div>
        </div>
       
    </div>
</template>

<style scoped>
#aboutmeSection {
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    height: 300px;
    margin-top: 400px;
}

.img-content img{
    width: 500px;
    border-radius: 8px;
    box-shadow: 1px 2px 8px #c97309;
}

.text-content {
    text-align: center;
}

.text-content h3{
    font-size: 50px;
    font-weight: bold
}

.text-content p {
    font-size: 23px;
    font-weight: bold;
}

.text-content span{
    color:#c97309;
}

.about-link {
    padding: 8px;
    border-radius: 8px;
    text-decoration: none;
    background-color: #c97309;
    color: #030755;
    font-weight: bold;
    cursor: pointer;
    box-shadow: 1px 2px 8px rgba(0, 0, 0, 0.233);
}

.text-content ul{
    margin-bottom: 30px;
}

.text-content li {
    font-size: 25px;
    text-align: left;
}

.nav-link img {
  width: 65px;
  margin-top: 50px;
  cursor: pointer;
  transition: transform 0.3s ease;
}

.nav-link img:hover {
    transform: scale(1.05);
}

.img-links {
    display: flex;
    align-items: center;
    justify-content: center;
}

@media (max-width: 768px) {
    #aboutmeSection{
        height: 50px;
        margin-top: 500px;
    }
    .img-content img {
        display: none;
    }
}

</style>