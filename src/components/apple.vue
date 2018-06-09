<template>
  <div>
    <h1>{{ msg }}</h1>
    <h1>{{ $route.params.color }}</h1>
    <button @click="getParam">get the router param</button>

  </div>
</template>

<script>
export default {
  data () {
    return {
      msg: 'Welcome to Your Apple'
    }
  },
  methods:{
    getParam(){
      console.log(this.$route.params);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
