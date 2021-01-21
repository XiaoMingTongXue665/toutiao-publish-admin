<template>
  <div id="app">
    <h1>黑马头条内容发布系统</h1>
    <el-row>
      <el-button>默认按钮</el-button>
      <el-button type="primary">主要按钮</el-button>
      <el-button type="success">成功按钮</el-button>
      <el-button type="info">信息按钮</el-button>
      <el-button type="warning">警告按钮</el-button>
      <el-button type="danger">危险按钮</el-button>
    </el-row>

    <el-input-number v-model="num" @change="handleChange" :min="10" :max="20" label="描述文字"></el-input-number>

    <!-- 路由出口 -->
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
      data() {
      return {
        num: 1
      };
    },
    methods: {
      handleChange(value) {
        console.log(value);
      }
    }
}

</script>

<style lang="less"></style>