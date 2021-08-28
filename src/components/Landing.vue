<template>
  <h1>{{content.title}}</h1>
  <img alt="civan erbay" class="landing-image" src="../assets/civan_erbay.png" /> 
  <button type="button" @click="count++">count is: {{ count }}</button>
</template>

<script>
  import contentJSON from '../content.js'
  export default {
    name: 'Landing',
    data() {
      return {
        count: 0,
        content: contentJSON,
      }
    }
  }
</script>

<style lang="scss" scoped>
  .landing-image {
    height: 50px;

  }
</style>