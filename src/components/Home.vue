<template>
  <div>
    <el-button type="info" @click="logout">推出</el-button>
  </div>
</template>

<script>
export default {
  methods: {
    logout() {
      // 清空缓存， 跳转到登录页
      window.sessionStorage.clear()
      this.$router.push('/login')
    }
  }
}
</script>

<style lang="less" scoped>
</style>