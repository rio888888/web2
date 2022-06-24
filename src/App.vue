<template>
  <div id="home">
    <img style="width: 100%; max-width: 750px;" src="./assets/images/1.png" alt="">
    <div class="links">
      <ul>
        <li @click="openLink('line')">
          <img style="max-width: 80px; max-height: 80px;" src="./assets/images/Line.png" alt="">
        </li>
        <li @click="openLink('whatsapp')">
          <img style="max-width: 80px; max-height: 80px;" src="./assets/images/WhatsApp.png" alt="">
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>

function openLink(type) {
  switch (type) {
    case 'line':
      console.log('line')
      window.location.href = 'https://line.me/ti/p/NSRiQJtG8_'
      break;

    case 'whatsapp':
      console.log('whatsapp')
      window.location.href = 'https://api.whatsapp.com/send/?phone=66631271873&text&app_absent=0'
      break;
  
    default:
      break;
  }
}
</script>

<style lang="scss">
body {
  margin: 0;
  font-size: 16px;
  text-align: center;
  ul {
    position: fixed;
    bottom: 30px;
    right: 20px;
    margin: 0;
    padding: 0;
    list-style: none;
    li {
      cursor: pointer;
      margin-bottom: 10px;
      img {
        width: 60px;
        height: 60px;
      }
    }
  }
}
</style>
