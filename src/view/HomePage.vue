<template>
    <div id="home">
        <MyHeader></MyHeader>
        <FirstSection></FirstSection>
        <AboutSection></AboutSection>
        <SecondSection></SecondSection>
        <ThirdSection></ThirdSection>
        <Footer></Footer>
    </div>
</template>

<script>
import MyHeader from '@/components/MyHeader.vue';
import FirstSection from '@/components/FirstSection.vue';
import AboutSection from '@/components/AboutSection.vue'
import SecondSection from '@/components/SecondSection.vue'
import ThirdSection from '@/components/ThirdSection.vue'
import Footer from '@/components/Footer.vue'

export default {
    name: 'homePage',
    components: {
        MyHeader,
        FirstSection,
        AboutSection,
        SecondSection,
        ThirdSection,
        Footer
    }
}

</script>