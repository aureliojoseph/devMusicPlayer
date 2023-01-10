<template>
  <div class="app__player--mini">
    <div class="player__mini">
      <div class="player__mini--info">
        <div class="mini-info">
          <img
            class="mini-image"
            alt="Band logo"
            src="../assets/pense-logo.jpeg"
          >
          <div class="mini__info--band">
            <p class="mini-song">Matrix</p>
            <p class="mini-band">Pense</p>
          </div>
        </div>
        <div class="player__mini--actions">
          <img src="../assets/chevron-left.svg" alt="chevron-left icon">
          <img src="../assets/caret-right.svg" alt="caret-right icon">
          <img src="../assets/chevron-right.svg" alt="chevron-right icon">
        </div>
      </div>
      <el-progress
        :stroke-width="4"
        :percentage="60"
        :show-text="false"
        >
        <span></span>
      </el-progress>
    </div>
  </div>
</template>

<script lang="ts">
  export default {
    name: 'AppPlayerMini'
  }
</script>

<style scoped>
  .app__player--mini {
    background: #0F0D13;
  }

  .player__mini {
    width: 390px;
    background: #854a4a;
    border-radius: 9px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 7px 7px 0;
  }

  .player__mini--info {
    display: flex;
    justify-content: space-between;
  }

  .mini-info {
    display: flex;
    align-items: center;
    gap: 12px;
  }

  .mini__info--band {
    display: flex;
    flex-direction: column;
    gap: 4px;
  }

  .mini-image {
    width: 86px;
    border-radius: 6px;
    margin-bottom: 6px;
  }

  .mini-song {
    font-weight: 700;
    font-size: 12px;
    color: #E1E1E6;
  }

  .mini-band {
    font-weight: 400;
    font-size: 10px;
    color: rgba(225, 225, 230, 0.6);
  }

  .player__mini--actions {
    display: flex;
    justify-content: center;
    gap: 18px;
    margin-bottom: 8px;
  }

  .player__mini--actions img {
    width: 20px;
    cursor: pointer;
    transition: all 0.3s;
  }
  
  .player__mini--actions img:hover {
    filter: invert(49%) sepia(16%) saturate(0%) hue-rotate(277deg) brightness(91%) contrast(91%);
  }

  :deep(.el-progress-bar__inner) {
    background-color: rgba(33, 53, 65, 0.6);
    transition: all 0.3s;
  }
  
  :deep(.el-progress-bar__inner:hover) {
    background-color: rgba(16, 26, 32, 0.8);
  }
</style>