<template>
  <div class="player__mini">
    <div>
      <img src="" alt="">
      <p>Musica Nome</p>
      <p>Banda Nome</p>
    </div>
    <div>
      <el-button>Play Back</el-button>
      <el-button>Play Pause</el-button>
      <el-button>Fast Forward</el-button>
    </div>
  </div>
</template>

<script lang="ts">
  export default {
    name: 'AppPlayerMini'
  }
</script>

<style scoped>
  .player__mobile {
    background: #0F0D13;
  }
</style>