<template>
  <div class="app__player--medium">
    <div class="player__medium">
      <div class="player__medium--info">
        <div class="medium-info">
          <img
            class="medium-image"
            alt="Band logo"
            src="../assets/propagandhi-logo.jpeg"
          >
          <div class="medium__info--band">
            <p class="medium-song">Victory Lap</p>
            <p class="medium-band">Propagandhi</p>
          </div>
        </div>
        <div class="player__medium--actions">
          <img src="../assets/chevron-left.svg" alt="chevron-left icon">
          <img src="../assets/caret-right.svg" alt="caret-right icon">
          <img src="../assets/chevron-right.svg" alt="chevron-right icon">
        </div>
        <div class="player__medium--time">
          <el-progress
            :stroke-width="8"
            :percentage="40"
            :show-text="false"
            >
            <span></span>
          </el-progress>
          <div class="medium-time">
            <p class="time-played">1:16</p>
            <p class="time-remaining">-1:40</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
  export default {
    name: 'AppPlayerMedium'
  }
</script>

<style scoped>
  .app__player--medium {
    background: #0F0D13;
  }

  .player__medium {
    width: 360px;
    background: #413721;
    border-radius: 9px;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .player__medium--info {
    padding: 38px;
  }

  .medium-info {
    display: flex;
    align-items: center;
    gap: 29px;
  }

  .medium__info--band {
    display: flex;
    flex-direction: column;
  }

  .medium-image {
    width: 84px;
    border-radius: 6px;
    margin-bottom: 29px;
  }

  .medium-song {
    font-weight: 700;
    font-size: 20px;
    color: #E1E1E6;
    margin-bottom: 10px;
  }

  .medium-band {
    font-weight: 400;
    font-size: 16px;
    color: rgba(225, 225, 230, 0.6);
    margin-bottom: 29px;
  }

  .player__medium--actions {
    display: flex;
    justify-content: center;
    gap: 50px;
    margin-bottom: 29px;
  }

  .player__medium--actions img {
    width: 28px;
    cursor: pointer;
    transition: all 0.3s;
  }
  
  .player__medium--actions img:hover {
    filter: invert(49%) sepia(16%) saturate(0%) hue-rotate(277deg) brightness(91%) contrast(91%);
  }

  :deep(.el-progress-bar__inner) {
    background-color: rgba(33, 53, 65, 0.6);
    transition: all 0.3s;
  }
  
  :deep(.el-progress-bar__inner:hover) {
    background-color: rgba(16, 26, 32, 0.8);
  }

  .medium-time {
    display: flex;
    justify-content: space-between;
    margin-top: 10px;
  }

  .medium-time p {
    font-size: 12px;
  }
</style>