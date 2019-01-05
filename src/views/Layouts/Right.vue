<template>
    <el-container>
        <el-header>
            <Nav></Nav>
        </el-header>
        <el-main>
            <Carousel></Carousel>
            <Content></Content>
        </el-main>
        <el-footer>
            <Footer></Footer>
        </el-footer>
    </el-container>
</template>

<script>
    // @ is an alias to /src
    import Nav from '@/components/Nav.vue'
    import Footer from '@/components/Footer.vue'
    import Content from '@/components/Content.vue'
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
    .el-header, .el-header {
        font-size: 12px;
        background-color: #409EFF;
        color: #606266;
        line-height: 60px;
    }
</style>

