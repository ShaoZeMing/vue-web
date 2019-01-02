<template>
    <el-carousel :interval="5000" arrow="arrow" height="400px">
        <el-carousel-item v-for="item in 4" :key="item">
            <img src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1547031579&di=048e85c76b58cd55de747a4a1b8ec01f&imgtype=jpg&er=1&src=http%3A%2F%2Fpic.97uimg.com%2Fback_pic%2F20%2F15%2F10%2F15%2F759683b9ac824b2b09f42d141d0e910b.jpg">
            <h3>Hello World</h3>
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

    .el-carousel__item:nth-child(2n) {
        background-color: #99a9bf;
    }

    .el-carousel__item:nth-child(2n+1) {
        background-color: #d3dce6;
    }
</style>
