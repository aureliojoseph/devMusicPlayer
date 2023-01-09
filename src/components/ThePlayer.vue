<template>
  <div class="the__player">
    <app-player-mobile />
    <div class="the__player--sizes">
      <!-- <app-player-medium />
      <app-player-mini /> -->
    </div>
  </div>
</template>

<script lang="ts">
  import AppPlayerMobile from './AppPlayerMobile.vue'
  import AppPlayerMedium from './AppPlayerMedium.vue'
  import AppPlayerMini from './AppPlayerMini.vue'

  export default {
    name: 'ThePlayer',
    components: {
      AppPlayerMobile,
      AppPlayerMedium,
      AppPlayerMini
    }
  }
</script>

<style scoped>
  .the__player {
    background: #0F0D13;
    border-radius: 8px 8px 8px 8px;
    padding: 50px 200px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
</style>