<template>
  <div id="app">
    <div class="app-header">
      <h2>do not bother me for fucking SQL....</h2>
      <img alt="Vue logo" src="./assets/avator.jpg" class="avator">
    </div>
    <div class="app-search">
      <el-input v-model="value" placeholder="随便输点什么，反正也没用..." style="width: 500px;margin-right: 20px"></el-input>
      <el-button @click="handleClick" type="primary">点一下</el-button>
    </div>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
  },

  data() {
    return {
      value: ''
    }
  },

  methods: {
    handleClick() {
      this.$message.success('反正就应该有点反应。。。')
    }
  },
}
</script>

<style>
.app-header {
  text-align: center;
}
.app-search {
  width: 100%;
  display: flex;
  justify-content: center;
}
.avator {
  height: 200px;
  width: 200px;
  object-fit: contain;
}
</style>
