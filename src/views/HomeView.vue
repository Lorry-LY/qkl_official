<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <FindUser msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import FindUser from '@/components/FindUser.vue'

export default {
  name: 'HomeView',
  components: {
    FindUser
  }
}
</script>
