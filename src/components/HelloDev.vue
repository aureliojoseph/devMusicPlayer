<template>
  <div class="hello__dev">
    <h1>Bem-vindos ao Dev Music Player!</h1>
    <h2>Um projeto <strong>#boracodar</strong> || 
      <a
        href="https://www.rocketseat.com.br/"
        rel="noopener"
        target="_blank"
        class="rocket-link"
        >@rocketseat
      </a>
    </h2>
    <h4>∞ Punk Mix ∞</h4>
    <div class="hello__dev--profile">
      <img src="../assets/profile.jpeg" alt="photo of Aurelio Borges">
      <div class="profile__info">
        <p>Aurelio Borges</p>
        <a
          href="https://www.linkedin.com/in/aurelioaborges/"
          rel="noopener"
          target="_blank"
          >@aurelioaborges
        </a>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
  export default {
    name: 'HelloDev'
  }
</script>

<style scoped>
  .hello__dev {
    padding: 40px;
    text-align: center;
  }

  .hello__dev h1,
  .hello__dev h2,
  .hello__dev h4 {
    margin-bottom: 24px;
  }

  h2 a {
    font-size: 18px;
    text-decoration: none;
    color: rgba(255, 255, 255, 0.64);
  }
  
  h2 a:hover {
    color: #fff;
  }

  h4 {
    color: #b3b3b3;
    transition: all .3s;
  }

  h4:hover {
    background: linear-gradient(to right, #21f34b, #ff8308, #23b2cf, #7d44ee);
    -webkit-text-fill-color: transparent;
    -webkit-background-clip: text;
  }

  .hello__dev--profile {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 16px;
  }

  img {
    width: 56px;
    border: 1px solid #fff;
    border-radius: 50%;
  }

  .profile__info {
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 8px;
  }

  .profile__info p {
    font-weight: 700;
    font-size: 18px;
    line-height: 12px;
    color: #E1E1E6;
  }

  .profile__info a {
    font-weight: 400;
    font-size: 14px;
    line-height: 8px;
    text-decoration: none;
    color: rgba(255, 255, 255, 0.639);
  }

  .profile__info a:hover {
    color: #fff;
  }
</style>