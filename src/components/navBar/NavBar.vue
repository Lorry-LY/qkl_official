<template>
  <el-menu
    :default-active="this.$router.path"
    class="el-menu-demo"
    mode="horizontal"
    :ellipsis="false"
    router
  >
    <div class="flex-grow" />
    <el-menu-item index="/">我们主页</el-menu-item>
    <div class="flex-grow" />
    <el-sub-menu index="2">
      <template #title>产品介绍</template>
      <el-menu-item index="2-1">item one</el-menu-item>
      <el-menu-item index="2-2">item two</el-menu-item>
      <el-menu-item index="2-3">item three</el-menu-item>
      <el-sub-menu index="2-4">
        <template #title>item four</template>
        <el-menu-item index="2-4-1">item one</el-menu-item>
        <el-menu-item index="2-4-2">item two</el-menu-item>
        <el-menu-item index="2-4-3">item three</el-menu-item>
      </el-sub-menu>
    </el-sub-menu>
    <el-sub-menu index="3">
      <template #title>产品支持</template>
      <el-menu-item index="3-1">item one</el-menu-item>
      <el-menu-item index="3-2">item two</el-menu-item>
      <el-menu-item index="3-3">item three</el-menu-item>
    </el-sub-menu>
    <div class="flex-grow" />
    <el-menu-item index="3" disabled>打开控制台</el-menu-item>
    <el-menu-item index="/login">登录</el-menu-item>
    <div class="flex-grow" />
  </el-menu>
</template>

<script>
export default {
  data () {
    return {

    }
  },
  components: {

  },
  created () {

  },
  methods: {

  }
}
</script>

<style scoped>
.flex-grow {
  flex-grow: 1;
}

.el-menu-demo{
  position:absolute;
  left: 0;
  top: 0;
  float: left;
  width: 100%;
  z-index: 1;
  background: transparent;
}
</style>
