<template>
  <div class="app__player--mobile">
    <div class="player__mobile">
      <div class="player__mobile--info">
        <img
          class="mobile-image"
          alt="Band logo"
          src="../assets/descendents-logo.jpeg"
        >
        <p class="mobile-song">When I Get Old</p>
        <p class="mobile-band">Descendents</p>
        <div class="player__mobile--actions">
          <img src="../assets/chevron-left.svg" alt="chevron-left icon">
          <img src="../assets/caret-right.svg" alt="caret-right icon">
          <img src="../assets/chevron-right.svg" alt="chevron-right icon">
        </div>
        <div class="player__mobile--time">
          <el-progress
            :stroke-width="8"
            :percentage="80"
            :show-text="false"
            >
            <span></span>
          </el-progress>
          <div class="mobile-time">
            <p class="time-played">2:06</p>
            <p class="time-remaining">-0:22</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
  export default {
    name: 'AppPlayerMobile'
  }
</script>

<style scoped>
  .app__player--mobile {
    background: #0F0D13;
  }

  .player__mobile {
    width: 270px;
    height: 498px;
    background: #213541;
    border-radius: 9px;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .player__mobile--info {
    padding: 38px;
  }

  .mobile-image {
    width: 190px;
    border-radius: 6px;
    margin-bottom: 29px;
  }

  .mobile-song {
    font-weight: 700;
    font-size: 20px;
    color: #E1E1E6;
    margin-bottom: 10px;
  }

  .mobile-band {
    font-weight: 400;
    font-size: 16px;
    color: rgba(225, 225, 230, 0.6);
    margin-bottom: 29px;
  }

  .player__mobile--actions {
    display: flex;
    justify-content: center;
    gap: 50px;
    margin-bottom: 29px;
  }

  .player__mobile--actions img {
    width: 28px;
    cursor: pointer;
    transition: all 0.3s;
  }
  
  .player__mobile--actions img:hover {
    filter: invert(49%) sepia(16%) saturate(0%) hue-rotate(277deg) brightness(91%) contrast(91%);
  }

  :deep(.el-progress-bar__inner) {
    background-color: rgba(33, 53, 65, 0.6);
    transition: all 0.3s;
  }
  
  :deep(.el-progress-bar__inner:hover) {
    background-color: rgba(16, 26, 32, 0.8);
  }

  .mobile-time {
    display: flex;
    justify-content: space-between;
    margin-top: 10px;
  }

  .mobile-time p {
    font-size: 12px;
  }
</style>