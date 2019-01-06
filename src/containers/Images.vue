<template>
        <el-row :gutter="24" justify="space-between">
            <el-col  :xs="24" :sm="24" :md="24" :lg="24" :xl="24">
                <div class="grid-content">
                    <el-row>
                        <h2>精选作品</h2>
                        <div class="line" >
                            <hr style="border-color: #d5d6d5">
                        </div>
                        <el-col :xs="12" :sm="8" :md="6" :lg="6" :xl="4"  v-for="(o, index) in 11" :key="o" :offset="index > 0 ? 0 : 0">
                            <div class="grid-content">
                                <block-card ></block-card>
                            </div>
                        </el-col>
                    </el-row>

                    <el-row>
                        <h2>热门作品</h2>
                        <div class="line" >
                            <hr style="border-color: #d5d6d5">
                        </div>
                        <el-col :xs="12" :sm="8" :md="6" :lg="6" :xl="4"  v-for="(o, index) in 11" :key="o" :offset="index > 0 ? 0 : 0">
                            <div class="grid-content">
                                <block-card ></block-card>
                            </div>
                        </el-col>
                    </el-row>
                </div>
            </el-col>
        </el-row>
</template>
<script>
    import BlockCard from '@/components/Card/BlockCard.vue'
    export default {
        name: 'Content',
        // props: {
        //     data: Object
        // },
        components: {
            BlockCard,
        },
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

    .el-row {
        margin-bottom: 20px;
    &:last-child {
         margin-bottom: 0;
     }
    }
    .el-col {
        border-radius: 4px;
    }
    /*.bg-purple-dark {*/
        /*background: #99a9bf;*/
    /*}*/
    /*.bg-purple {*/
        /*background: #d3dce6;*/
    /*}*/
    /*.bg-purple-light {*/
        /*background: #e5e9f2;*/
    /*}*/
    .grid-content {
        border-radius: 4px;
        min-height: 36px;
    }
    /*.row-bg {*/
        /*padding: 10px 0;*/
        /*background-color: #f9fafc;*/
    /*}*/
    .image {
        border-radius: 4px;
        width: 100%;
        display: block;
    }
</style>
