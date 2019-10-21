<template>
  <div>
    <span class="mian">hello world</span>
    <van-button type="primary" @click="jump">按钮</van-button>
  </div>
</template>

<script>
  import { post } from '../../utils/request'

  export default {
    methods: {
      jump() {
        post('https://www.baidu.com').then(response => {
          console.log('handleResponse....')
        })
      }
    }
  }
</script>

<style lang="stylus" scoped>
  .mian {
    color: red;
    font-size: 20px;
    font-weight: bold;
  }
</style>
