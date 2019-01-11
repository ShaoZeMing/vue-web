<template>
    <el-container>
        <el-header>
            <Nav></Nav>
        </el-header>
        <el-main>
            <Carousel></Carousel>
            <Content></Content>
        </el-main>
        <el-footer height="200">
            <Footer></Footer>
        </el-footer>
    </el-container>
</template>

<script>
    // @ is an alias to /src
    import Nav from '@/containers/Nav.vue'
    import Footer from '@/containers/Footer.vue'
    import Content from '@/containers/Content.vue'
    import Carousel from '@/components/Carousel.vue'


    export default {
        name: 'home',
        components: {
            Nav,
            Footer,
            Content,
            Carousel,
        }
    }
</script>


<style>
.el-main{
    margin-top: 60px;
}


</style>

