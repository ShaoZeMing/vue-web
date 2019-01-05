<template>
    <el-carousel :interval="5000" arrow="arrow"  class="hidden-xs-only">
        <el-carousel-item v-for="item in 4" :key="item">
            <!--<h3>Hello World</h3>-->
            <img src="https://img.zcool.cn/community/01af5f58258bb6a84a0e282b7e9d53.jpg@2o.jpg" class="image">
        </el-carousel-item>
    </el-carousel>
</template>
<script>
    export default {
        name: 'Carousel',
        // props: {
        //     data: Object
        // },
        data() {

            const item = {
                date: '2016-05-02',
                name: '王小虎',
                address: '上海市普陀区金沙江路 1518 弄'
            };
            return {
                tableData: Array(20).fill(item)
                // tableData: this.props.data
            }
        }
    };
</script>

<style>
    .el-carousel__item h3 {
        color: #475669;
        font-size: 18px;
        opacity: 0.75;
        line-height: 300px;
        margin: 0;
    }

    /*.image {*/
        /*!*width: 100%;*!*/
        /*!*display: block;*!*/
    /*}*/
    .el-carousel__item:nth-child(2n) {
        background-color: #99a9bf;
    }

    .el-carousel__item:nth-child(2n+1) {
        background-color: #d3dce6;
    }
</style>
