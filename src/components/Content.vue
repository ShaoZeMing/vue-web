<template>
        <el-row :gutter="24">
            <el-col :span="16">
                <div class="grid-content">
                    <el-row>
                        <el-col :span="6" v-for="(o, index) in 11" :key="o" :offset="index > 0 ? 0 : 0">
                            <div class="grid-content">
                                <Card ></Card>
                            </div>
                        </el-col>
                    </el-row>
                </div>
            </el-col>
            <el-col :span="8" style="text-align: left">
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
                       <img src="http://mijia365.oss-cn-beijing.aliyuncs.com/mijia-categories/IMG_51521546408986142.PNG" style="width: 400px;">
                        </div>
                    </el-col>
                </el-row>
                <el-row :gutter="24">
                    <el-col :span="24">
                        <div class="grid-content">
                        <h2>周排行榜</h2>
                        <!--<img src="http://mijia365.oss-cn-beijing.aliyuncs.com/mijia-categories/IMG_51521546408986142.PNG">-->
                        </div>
                    </el-col>
                </el-row>
                <el-row :gutter="24">
                    <el-col :span="24">
                        <div class="grid-content">
                        <h2>专题</h2>
                            <img src="http://mijia365.oss-cn-beijing.aliyuncs.com/mijia-categories/IMG_51521546408986142.PNG" style="width: 400px;">
                        </div>
                    </el-col>
                </el-row>
                </div>
            </el-col>
        </el-row>
</template>
<script>
    import Card from '@/components/Card.vue'
    export default {
        name: 'Content',
        // props: {
        //     data: Object
        // },
        components: {
            Card,
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

