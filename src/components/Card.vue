<template>
  <el-card :body-style="{ padding: '0px' }" shadow="hover">
    <img src="http://element-cn.eleme.io/static/hamburger.50e4091.png" class="image">
    <div style="padding: 14px;">
      <span>好吃的汉堡</span>
      <div class="bottom clearfix">
        <time class="time">{{ currentDate }}</time>
        <el-button type="text" class="button">操作按钮</el-button>
      </div>
    </div>
  </el-card>
</template>

<script>
export default {
  name: 'Card',
  // props: {
    // work: Object
  // }

    data() {
        return {
            currentDate: new Date()
        };
    }
}
</script>


<style>
  .time {
    font-size: 13px;
    color: #999;
  }

  .bottom {
    margin-top: 13px;
    line-height: 12px;
  }

  .button {
    padding: 0;
    float: right;
  }

  .image {
    width: 100%;
    display: block;
  }

  .clearfix:before,
  .clearfix:after {
    display: table;
    content: "";
  }

  .clearfix:after {
    clear: both
  }
  .el-card{
    margin-top: 20px;
    margin-right: 20px;
  }
</style>

