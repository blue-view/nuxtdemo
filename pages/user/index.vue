<template>
  <div>
    <nuxt-link to="/user/5">详情页</nuxt-link>
    <el-button type="primary" @click="say">查询</el-button>
    
  </div>
</template>

<script>
export default {
  asyncData({app}) {
    console.log(app.sort([1,3,4,5,6]))
    console.log(app.$integerSort([3,4,2,4,5]))
  },
  methods: {
    say(){
    this.$debug('hello')
     console.log(this.$integerSort([3,9,2,4,5]))
    }
  }
};
</script>

<style lang="scss" scoped></style>
