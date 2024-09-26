<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    
    <div class="wrapper">
      <div class="main-card">
        <div class="head">
          <div class="img">
            <img src="./assets/img/ava.jpg" alt="avatar">
          </div>
          <div class="name">
            <h2>Sarvarbek Sadilloyev</h2>
            <p>Uzbekistan, Kashkadarya</p>
          </div>
          <p class="job">
            "Front-end developer and Designer"
          </p>
        </div>
        <div class="link">
          <div class="section">
            <RouterLink to="/main" class="section">Main Website</RouterLink>
          </div>
          <div class="section">
            <RouterLink to="/" class="section">Instagram</RouterLink>
          </div>
          <div class="section">
            <RouterLink to="/" class="section">Telegram</RouterLink>
          </div>
          <div class="section">GitHub</div>
          <div class="section">
            <RouterLink to="/" class="section">CodeWars</RouterLink>
          </div>
          <!-- <RouterLink to="/" class="section">Home</RouterLink>
          <RouterLink to="/about" class="section">About</RouterLink> -->
        </div>
      </div>
      
    </div>
  </header>
  
  <RouterView />
</template>

<style lang="scss" scoped>
header {
  .wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 auto;
    height: 100vh;
    
    .main-card {
      display: flex;
      flex-direction: column;
      align-items: center;
      height: 60%;
      background-color: #1F1F1F;
      padding: 20px;
      border-radius: 15px;
      .head {
        display: flex;
        flex-direction: column;
        align-items: center;
        .img {
          width: 100px;
          height: 100px;
          
          img {
            width: 100%;
            height: 100%;
            border-radius: 50%;
          }
        }
        
        .name {
          padding: 10px;
          text-align: center;
          h2 {
            color: #FFF;
          }
          p {
            padding-top: 5px;
            color: #C5F82A;
          }
        }
        
        .job {
          padding: 15px 0;
          color: #9B9B9B;
        }
      }

      .link {
        display: flex;
        flex-direction: column;
        gap: 10px;

        .section {
          display: flex;
          flex-direction: column;
          justify-content: center;
          width: 200px;
          height: 30px;
          background-color: #333;
          color: #fff;
          font-size: 20px;
          text-align: center;
          border-radius: 10px;
        }
      }
    }
  }
}
</style>
