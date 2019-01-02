<template>
    <el-container direction="vertical">
        <Header></Header>
        <Carousel></Carousel>
        <el-main>
            <Content></Content>
        </el-main>
        <Footer></Footer>
    </el-container>
</template>

<script>
    // @ is an alias to /src
    import Header from '@/components/Header.vue'
    import Footer from '@/components/Footer.vue'
    import Content from '@/components/Content.vue'
    import Carousel from '@/components/Carousel.vue'


    export default {
        name: 'home',
        components: {
            Header,
            Footer,
            Content,
            Carousel,
        }
    }
</script>


