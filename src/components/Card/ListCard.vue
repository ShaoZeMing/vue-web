<template>
  <el-card :body-style="{ padding: '2%' }" shadow="hover">
    <el-col :span="8" >
      <div class="grid-content">
        <img src="http://element-cn.eleme.io/static/hamburger.50e4091.png" class="image-card-list">
      </div>
    </el-col>
    <el-col :span="16" >
      <div class="grid-content">
        <div class="card-list-content">
          <span>好吃的汉堡</span>
          <div>
            <time class="time">创建时间:{{ currentDate }}</time>
            <el-button type="text" class="button">操作按钮</el-button>
          </div>
        </div>
      </div>
    </el-col>
  </el-card>
</template>

<script>
export default {
  name: 'ListCard',
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

  /*.bottom {*/
    /*margin-top: 13px;*/
    /*line-height: 12px;*/
  /*}*/

  /*.button {*/
    /*padding: 0;*/
    /*float: right;*/
  /*}*/

  .image-card-list {
    width: 80%;
    display: inline;
    border-radius: 4px;
    border: 1px solid #ebeef5;
    overflow: hidden;
    /*margin-top: 10px;*/
  }

  .card-list-content{
    /*margin-top: 10px;*/
  }
  .clearfix:before,
  .clearfix:after {
    display: table;
    content: "";
  }

  .clearfix:after {
    clear: both
  }
</style>

