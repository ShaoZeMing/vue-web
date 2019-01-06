<template>
    <el-container>
        <el-header>
            <Nav></Nav>
        </el-header>
        <el-main>
            <Images></Images>
        </el-main>
        <el-footer>
            <Footer></Footer>
        </el-footer>
    </el-container>
</template>

<script>
    // @ is an alias to /src
    import Nav from '@/containers/Nav.vue'
    import Footer from '@/containers/Footer.vue'
    import Images from '@/containers/Images.vue'


    export default {
        name: 'home',
        components: {
            Nav,
            Footer,
            Images,
        }
    }
</script>


<style>
.el-main{
    margin-top: 60px;
}


</style>

