<template>
  <section class="section1">
    <div class="div-section1 width80pr">
      <div class="section1-img" v-for="game in gameType" :key="game.title">
        <img :src="game.image" :alt="game.title" />
        <p class="hidden-text">{{ game.title }}</p>
        <p class="item-name">{{ game.subTitle }}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "gameType-item",

  data: () => ({
    gameType: [
      {
        title: "PLAY FOR SPORTS",
        subTitle: "Sports",
        image: require("@/assets/section1-img1.png"),
      },
      {
        title: "PLAY FOR LIVE",
        subTitle: "Live casino",
        image: require("@/assets/section1-img2.png"),
      },
      {
        title: "PLAY FOR E-GAMES",
        subTitle: "E-games",
        image: require("@/assets/section1-img3.png"),
      },
      {
        title: "PLAY FOR CHESS",
        subTitle: "Chess games",
        image: require("@/assets/section1-img4.png"),
      },
    ],
  }),
};
</script>

<style scoped>
  .section1 {
    background: url(@/assets/section-bg.png);
    background-size: cover;
    background-position: -195px 0px;
    background-repeat: no-repeat;
    background-color: #000c;
    width: 100%;
    height: 419px;
  }

  .div-section1 {
    display: flex;
    justify-content: space-between;
    padding-top: 30px;
  }
  .section1-img {
    position: relative;
    cursor: pointer;
  }

  .hidden-text {
    width: 202px;
    line-height: 51px;
    text-align: center;
    font-size: 16px;
    font-family: "Adobe Heiti Std";
    color: #ebc86d;
    background: #0000008c;
    border-radius: 8px;
    border: 1px solid #ebc86d;
    position: absolute;
    top: 50%;
    left: 50%;
    margin-left: -101px;
    display: none;
  }
  .section1-img:hover img {
    filter: grayscale(0.6);
  }
  .section1-img:hover .hidden-text {
    display: block;
  }

  .item-name {
    width: 143px;
    height: 51px;
    background: url(@/assets/item-name.png);
    font-size: 19px;
    color: #712213;
    font-style: italic;
    justify-content: center;
    text-align: center;
    line-height: 51px;
    position: absolute;
    bottom: -35px;
    right: 0;
    z-index: 1;
    display: flex;
    align-items: center;
  }
</style>
