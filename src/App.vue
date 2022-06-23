<template>
  <div id="home">
    <img @click="openLink" style="width: 100%;" src="./assets/images/1.png" alt="">
    <div class="links">
      <ul>
        <li>
          <img src="./assets/images/Line.png" alt="">
        </li>
        <li>
          <img src="./assets/images/WhatsApp.png" alt="">
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
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
