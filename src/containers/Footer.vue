<template>
    <el-row :gutter="10" type="flex" class="footer" justify="space-between">
        <el-col :xs="12" :sm="10" :md="8" :lg="6" :xl="3">
            <div class="grid-content ">
                    <dl>
                        <dd>  <a href="#">关于我们</a></dd>
                        <dd>  <a href="#">关于我们</a></dd>
                        <dd>  <a href="#">关于我们</a></dd>
                    </dl>
            </div>
        </el-col>
        <el-col :xs="12" :sm="10" :md="8" :lg="6" :xl="3">
            <div class="grid-content ">
                <dl>
                    <dd>  <a href="#">关于我们</a></dd>
                    <dd>  <a href="#">关于我们</a></dd>
                    <dd>  <a href="#">关于我们</a></dd>
                </dl>
            </div>
        </el-col>
    </el-row>
</template>
<script>
    export default {
        name: 'Footer',
        // props: {
        //   user: Object
        // }
    }
</script>


<style>
    .footer {
        margin-top: 15px;
    }

    .el-footer {
        text-align: left;
        font-size: 0.9em;
        background-color: #409EFF;
        color: #303133;
        line-height: 30px;
    }


    .grid-content {
        border-radius: 4px;
        min-height: 36px;
    }
</style>
