<template>
    <!--<el-header>-->
    <!--<el-row :gutter="10">-->
    <el-menu
            :default-active="activeIndex2"
            class="el-menu-demo"
            mode="horizontal"
            @select="handleSelect"
            background-color="#409EFF"
            text-color="#fff"
            active-text-color="#ffd04b">
        <el-col :span="4"><div class="grid-content bg-purple">
            <img src="http://mijia-web.4d4k.com/images/logo.png"/>
        </div></el-col>
        <el-col :span="3"><div class="grid-content bg-purple">
            <el-menu-item index="1"><a href="/" target="_blank">首页</a></el-menu-item></div>
        </el-col>
        <el-col :span="3">
            <div class="grid-content bg-purple">
            <el-submenu index="2">
                <template slot="title">发现</template>
                <el-menu-item index="2-1">选项1</el-menu-item>
                <el-menu-item index="2-2">选项2</el-menu-item>
                <el-menu-item index="2-3">选项3</el-menu-item>
                <el-submenu index="2-4">
                    <template slot="title">选项4</template>
                    <el-menu-item index="2-4-1">选项1</el-menu-item>
                    <el-menu-item index="2-4-2">选项2</el-menu-item>
                    <el-menu-item index="2-4-3">选项3</el-menu-item>
                </el-submenu>
            </el-submenu>
        </div>
        </el-col>
        <el-col :span="3">
            <div class="grid-content bg-purple">
                <el-menu-item index="3" disabled>问答</el-menu-item>
            </div>
        </el-col>
        <el-col :span="3">
            <div class="grid-content bg-purple">
                <el-menu-item index="3" disabled>下载</el-menu-item>
            </div>
        </el-col>
        <el-col :span="3">
            <div class="grid-content bg-purple">
                <el-menu-item index="3" disabled>搜索</el-menu-item>
            </div>
        </el-col>
        <el-col :span="4" :offset="1" >
            <div class="grid-content bg-purple">
                <el-submenu index="5">
                    <template slot="title">
                        <img src="http://img4.duitang.com/uploads/item/201210/07/20121007194928_whKNM.jpeg" style="width: 30px;display: inline">
                        小明
                    </template>
                    <el-menu-item index="5-1">选项1</el-menu-item>
                    <el-menu-item index="5-2">选项2</el-menu-item>
                    <el-menu-item index="5-3">选项3</el-menu-item>
                </el-submenu>
            </div>
            </el-col>
    </el-menu>

    <!--</el-row>-->


    <!--<el-dropdown>-->
    <!--<i class="el-icon-setting" style="margin-right: 15px"></i>-->
    <!--<el-dropdown-menu slot="dropdown">-->
    <!--<el-dropdown-item>查看</el-dropdown-item>-->
    <!--<el-dropdown-item>新增</el-dropdown-item>-->
    <!--<el-dropdown-item>删除</el-dropdown-item>-->
    <!--</el-dropdown-menu>-->
    <!--</el-dropdown>-->
    <!--<span>王小虎</span>-->
    <!--</el-header>-->
</template>

<script>


    export default {
        name: 'Header',
        data() {
            return {
                activeIndex: '1',
                activeIndex2: '1'
            };
        },
        methods: {
            handleSelect(key, keyPath) {
                console.log(key, keyPath);
            }
        }
    }
</script>


<style>
    .el-header {
        font-size: 12px;
        background-color: #409EFF;
        color: #606266;
        line-height: 60px;
    }

    .el-dropdown {
        align-content: right;
    }
</style>
