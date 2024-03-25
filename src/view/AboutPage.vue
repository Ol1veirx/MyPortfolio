<template>
    <div id="Myabout">
        <MyHeader></MyHeader>
        <MyAbout></MyAbout>
    </div>
</template>

<script>
import MyHeader from '@/components/MyHeader.vue';
import MyAbout from '@/components/MyAbout.vue'

export default {
    name: 'aboutPage',
    components: {
        MyHeader,
        MyAbout,
    }
}
</script>