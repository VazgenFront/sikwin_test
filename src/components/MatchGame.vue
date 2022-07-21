<template>
  <section class="section2 width80pr">
    <div class="secttion2-left">
      <div class="e-games">
        <div class="e-games-logo">
          <img src="@/assets/section2-img1.png" alt="" />
        </div>
        <div class="e-games-txt">
          <p>MG SLOT</p>
          <span>E-GAMES</span>
        </div>
      </div>
      <div class="e-games">
        <div class="e-games-logo">
          <img src="@/assets/section2-img2.png" alt="" />
        </div>
        <div class="e-games-txt">
          <p>MG SLOT</p>
          <span>E-GAMES</span>
        </div>
      </div>
    </div>
    <div class="section2-right">
      <div class="image">
        <img src="@/assets/section2-img3.png" alt="" />
      </div>
      <div class="btn">Bet now</div>
    </div>
  </section>
</template>

<script>
  export default {
    name: "matchGame-item",
  };
</script>

<style scoped>
  .section2 {
    width: 1200px;
    margin: 0 auto;
    display: flex;
  }

  .e-games {
    width: 422px;
    height: 180px;
    padding: 45px 0 47px 40px;
    display: flex;
    align-items: center;
    background: #00000072;
    cursor: pointer;
  }
  .e-games-logo {
    width: 112px;
    margin-right: 30px;
  }
  .e-games-logo img {
    width: 100%;
  }
  .e-games-txt {
    line-height: 42px;
    margin-top: 10px;
    color: #cbcbcb;
    font-style: italic;
  }

  .e-games-txt p {
    font-size: 30px;
  }
  .e-games-txt span {
    font-size: 16px;
  }
  .image {
    padding: 30px 0px 0px 30px;
  }

  .btn {
    margin: 0 auto;
    margin-top: 60px;
    width: 272px;
    text-align: center;
    line-height: 55px;
    font-style: italic;
    font-size: 22px;
    color: #ffcf51;
    background: #00000063;
    border-radius: 8px;
    border: 2px solid #ffcf51;
    cursor: pointer;
    margin-bottom: 20px;
  }
  .e-games:hover {
    background: #fbfbfb2e;
  }
  .e-games:hover .e-games-txt {
    color: #e17f00;
  }
</style>
