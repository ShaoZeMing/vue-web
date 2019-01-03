<template>
        <el-row :gutter="24" justify="space-between">
            <el-col  :xs="24" :sm="24" :md="16" :lg="16" :xl="16">
                <div class="grid-content">
                    <el-row>
                        <h2>精选作品</h2>
                        <div class="line" >
                            <hr style="border-color: #d5d6d5">
                        </div>
                        <el-col :xs="12" :sm="8" :md="6" :lg="6" :xl="4"  v-for="(o, index) in 11" :key="o" :offset="index > 0 ? 0 : 0">
                            <div class="grid-content">
                                <Card ></Card>
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
                                <Card ></Card>
                            </div>
                        </el-col>
                    </el-row>
                </div>
            </el-col>
            <el-col  :xs="24" :sm="24" :md="8" :lg="8" :xl="8"  style="text-align: left">
                <div class="grid-content">
                <el-row :gutter="24">
                    <el-col :span="24">
                        <div class="grid-content">

                        <h2>少儿为什么学习编程</h2>
                        <p>注册一个帐户以管理、分享您的作品，并跟踪你的进度，作为老师，可以更快捷、高效地管理您的教室。</p>
                        <p>让我们开始编程吧！</p>
                        </div>
                    </el-col>
                </el-row>
                <el-row :gutter="24">
                    <el-col :span="24">
                        <div class="grid-content">
                        <h2>推荐</h2>
                       <img src="http://mijia365.oss-cn-beijing.aliyuncs.com/mijia-categories/IMG_51521546408986142.PNG" class="image">
                        </div>
                    </el-col>
                </el-row>
                <el-row :gutter="24">
                    <el-col :span="24">
                        <div class="grid-content">
                        <h2>周排行榜</h2>
                            <el-row :gutter="24" v-for="o in 5" :key="o" >
                                <el-col :span="24" >
                                    <div class="grid-content">
                                        <card-list ></card-list>
                                    </div>
                                </el-col>
                            </el-row>
                        </div>
                    </el-col>
                </el-row>
                <el-row :gutter="24">
                    <el-col :span="24">
                        <div class="grid-content">
                        <h2>专题</h2>
                            <img src="http://mijia365.oss-cn-beijing.aliyuncs.com/mijia-categories/IMG_51521546408986142.PNG" class="image">
                        </div>
                    </el-col>
                </el-row>
                </div>
            </el-col>
        </el-row>
</template>
<script>
    import Card from '@/components/Card.vue'
    import CardList from '@/components/CardList.vue'
    export default {
        name: 'Content',
        // props: {
        //     data: Object
        // },
        components: {
            Card,
            CardList,
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
