<template>
  <div class="app">
    <Navbar />
    <Slider />
    <GameTypes />
    <MatchGame />
    <EntertainmentGame />
  </div>
</template>

<script>
  import Navbar from "@/components/Navbar.vue";
  import Slider from "@/components/Slider.vue";
  import GameTypes from "@/components/GameTypes.vue";
  import MatchGame from "@/components/MatchGame.vue";
  import EntertainmentGame from "@/components/EntertainmentGame.vue";

  export default {
    name: "App",
    components: {
      Navbar,
      Slider,
      GameTypes,
      MatchGame,
      EntertainmentGame,
    },
  };
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    background-repeat: no-repeat;
    background-size: cover;
  }
  .app {
    background: url(@/assets/background.png) 50% no-repeat;
  }
  a {
    text-decoration: none;
  }
  a:hover {
    text-decoration: none;
  }

  .width80pr {
    width: 80%;
    margin: 0 auto;
  }
</style>
