<template>
<div class="holder">
    <div class="first"></div>
    <div class="second"></div>
    <div class="third"></div>
  <div id="app">
    <img src="./assets/logo.png">
    <router-view/>
  </div>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
  @import url(https://fonts.googleapis.com/css?family=Bitter);
    body {
      margin: 0;
      font-family: 'Bitter', serif;
      text-align: center;
    }
    .holder,
    .first,
    .second,
    .third {
      height: 100vh;
      width: 100vw;
    }
    .first,
    .second,
    .third {
      position: absolute;
    }
    .second,
    .third {
      opacity: 0;
    }
    .holder {
      height: 100vh;
      position: relative;
      z-index: 1;
    }
    .first {
      animation: first 10s infinite;
      background: linear-gradient(#ff7f50, #60e08c);
      z-index: 10;
    }
      @keyframes first {
        0% {opacity: 1.0;}
        10% {opacity: 0.8;}
        20% {opacity: 0.6;}
        30% {opacity: 0.4;}
        40% {opacity: 0.2;}
        50% {opacity: 0.1;}
        60% {opacity: 0.2;}
        70% {opacity: 0.4;}
        80% {opacity: 0.6;}
        90% {opacity: 0.8;}
        100% {opacity: 1.0;}
      }

    .second {
      animation: second 10s infinite; animation-delay: 2s;
      background: linear-gradient(#19eaa6, #00a1f0);
      z-index: 20;
    }
      @keyframes second {
        0% {opacity: 0;}
        10% {opacity: 0.2;}
        20% {opacity: 0.4;}
        30% {opacity: 0.6;}
        40% {opacity: 0.8;}
        50% {opacity: 1.0;}
        60% {opacity: 0.8;}
        70% {opacity: 0.6;}
        80% {opacity: 0.4;}
        90% {opacity: 0.2;}
        100% {opacity: 0;}
      }

    .third {
      animation: third 10s infinite;
      animation-delay: 8s;
      background: linear-gradient(#aab7f8, #ffc44f);
      z-index: 30;
    }
      @keyframes third {
        0% {opacity: 0;}
        10% {opacity: 0.2;}
        20% {opacity: 0.4;}
        30% {opacity: 0.6;}
        40% {opacity: 0.8;}
        50% {opacity: 1.0;}
        60% {opacity: 0.8;}
        70% {opacity: 0.6;}
        80% {opacity: 0.4;}
        90% {opacity: 0.2;}
        100% {opacity: 0;}
      }
      #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        padding-top: 60px;
        z-index:1000;
        position: relative;
        }
      img{
          border-radius:20%;
          width:180px;
          height:180px;
          object-fit: cover;
          }

</style>
