<template>
  <div class="home">
    <div class="rotate">
      <img class="circle_1" src="../assets/circle_1.svg" alt="circle_1">
      <img class="circle_2" src="../assets/circle_2.svg" alt="circle_2">
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Home',
    components: {}
  }
</script>

<style lang="scss">
  .circle_1 {
    right: 300px;
    bottom: 300px;
    position: absolute;
    -webkit-animation: spin 10s linear infinite;
    -moz-animation: spin 10s linear infinite;
    animation: spin 10s linear infinite;
  }

  .circle_2 {
    position: absolute;
    -webkit-animation: spin 20s linear infinite;
    -moz-animation: spin 20s linear infinite;
    animation: spin 20s linear infinite;
  }

  @-moz-keyframes spin {
    100% {
      -moz-transform: rotate(360deg);
    }
  }

  @-webkit-keyframes spin {
    100% {
      -webkit-transform: rotate(360deg);
    }
  }

  @keyframes spin {
    100% {
      -webkit-transform: rotate(360deg);
      transform: rotate(360deg);
    }
  }
</style>