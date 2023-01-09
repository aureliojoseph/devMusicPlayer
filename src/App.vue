<template>
  <div>
    <hello-dev />
    <the-player />
  </div>
</template>

<script lang="ts">
  import HelloDev from './components/HelloDev.vue'
  import ThePlayer from './components/ThePlayer.vue'
  
  export default {
    name: 'App',
    components: {
      HelloDev,
      ThePlayer
    }
  }
</script>

<style scoped>

</style>