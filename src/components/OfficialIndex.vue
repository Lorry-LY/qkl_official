<template>
  <div class="content">
    <el-row>
      <el-col :span="12">
        <div class="grid-content bg-purple">
          <div class="text">
            <div class="title">
              Cool & Amazing Landing Page
            </div>
            <div class="introduce">
              Itaque earum rerum tenetur sapiente delectus ut aut reiciendis voluptatibus maiores alias consequatur repellat.
            </div>
            <el-button  class="btn" type="primary">加入我们</el-button>
            <!-- <div class="vedio_content">
              <el-button class="btn1" :icon="Search" circle />
              查看详细介绍
            </div> -->
          </div>
        </div>
      </el-col>
      <el-col :span="12">
        <div class="grid-content bg-purple-light">
          <!-- <el-image fit="fill" placeholder="图片正在加载。。" error="图片加载失败" key="index.png" src="../assets/index.png" alt="我的图片不在了" lazy></el-image> -->
          <img class="image" placeholder="图片正在加载" src="../assets/index.png" />
        </div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  data () {
    return {
      name: 1
    }
  },
  methods: {

  }
}
</script>

<style lang="less" scoped>
  .content {
    position : absolute;
    width : 100%;
    height : 100%;
  }
  .el-row {
    height: 100%;
    margin-bottom: 20px;
    &:last-child {
      margin-bottom: 0;
    }
  }

  .btn {
    position:absolute;
    width: 160px;
    height: 60px;
    background: #5a4fdc;
    left: 5%;
    margin: 30px auto;
  }

  .btn1 {
    position:absolute;
    width: 80px;
    height: 80px;
    left: 5%;
    background: transparent;
    border-block: #000;
  }

  .vedio_content {
    padding-top: 40%;
    width: 100%;
    text-align: left;
  }

  .text {
    position: absolute;
    width: 60%;
    height: 70%;
    top: 20%;
    left: 0;
    right: -30%;
    bottom: 0;
    margin: auto;
  }

  .title {
    font-size: 3em;
    margin: 30px auto;
    text-align: left;
  }

  .introduce {
    font-size: 1em;
    margin: 30px auto;
    text-align: left;
  }

  .image{
    position: absolute;
    width: 80%;
    height: 100%;
    top: 0;
    left: -10%;
    right: 0;
    bottom: 0;
    margin: auto;
  }
  .el-col {
    border-radius: 4px;
  }
  .bg-purple-dark {
    background: transparent;
  }
  .bg-purple {
    background: transparent;
  }
  .bg-purple-light {
    background: transparent;
  }
  .grid-content {
    position: relative;
    border-radius: 4px;
    min-height: 36px;
    height: 100%;
  }
</style>
