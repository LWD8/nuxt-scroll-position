<template>
  <div>
    <p>跳转过来了，id值为{{$route.query.id}}</p>
    <p @click="aa">返回首页》</p>
  </div>
</template>

<script>
  export default {
    methods: {
      aa() {
        this.$router.go(-1)
        // this.$router.push({name: 'index'})
      }
    }
  }
</script>