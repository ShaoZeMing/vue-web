<template>
    <el-row :gutter="10" type="flex" class="footer" justify="space-between">
        <el-col :xs="12" :sm="10" :md="8" :lg="6" :xl="3">
            <div class="grid-content bg-purple"></div>
        </el-col>
        <el-col :xs="12" :sm="10" :md="8" :lg="6" :xl="3">
            <div class="grid-content bg-purple-light"></div>
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
        text-align: right;
        font-size: 12px;
        background-color: #409EFF;
        color: #303133;
        line-height: 120px;
    }

    .bg-purple-dark {
        background: #99a9bf;
    }

    .bg-purple {
        background: #d3dce6;
    }

    .bg-purple-light {
        background: #e5e9f2;
    }

    .grid-content {
        border-radius: 4px;
        min-height: 36px;
    }
</style>
