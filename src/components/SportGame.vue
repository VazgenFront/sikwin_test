<template>
  <section class="section4">
    <div class="center-img">
      <img src="@/assets/center-img.png" alt="" />
    </div>

    <div class="sport-game-center width80pr">
      <div class="left-side">
        <div class="left-side-top">
          <img src="@/assets/section4-img1.png" alt="" />
        </div>
        <div class="left-side-btm">
          <img src="@/assets/section4-img2.jpg" alt="" />
        </div>
      </div>
      <div class="right-side">
        <div class="right-side-top">
          <img src="@/assets/section4-img3.png" alt="" />
        </div>
        <div class="right-side-mid">
          <img src="@/assets/section4-img4.jpg" alt="" />
        </div>
        <div class="right-side-btm">
          <img src="@/assets/section4-img5.png" alt="" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "sportGame-item",
};
</script>

<style>
.section4 {
  width: 100%;
  height: 720px;
  overflow: hidden;
  position: relative;
}

.center-img {
  height: 720px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background: url(@/assets/center-img-bg.png) no-repeat;
  z-index: 1;
}

.sport-game-center {
  position: relative;
  display: flex;
  justify-content: space-between;
}
.left-side-top {
  height: 425px;
  padding-left: 20px;
  display: flex;
  align-items: center;
  cursor: pointer;
}

.left-side-btm {
  width: 306px;
  height: 296px;
  padding-left: 20px;
  display: flex;
  align-items: center;
  cursor: pointer;
}
.right-side {
  z-index: 0;
}
.right-side-top {
  padding-right: 30px;
  height: 255px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  cursor: pointer;
}
.right-side-mid {
  padding-right: 30px;
  height: 245px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  cursor: pointer;
}
.right-side-btm {
  padding-right: 30px;
  height: 245px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  cursor: pointer;
}

.left-side-top img,
.left-side-btm img,
.right-side-top img,
.right-side-mid img,
.right-side-btm img {
  transition: 0.5s;
}

.left-side-top img:hover,
.left-side-btm img:hover,
.right-side-top img:hover,
.right-side-mid img:hover,
.right-side-btm img:hover {
  transform: translateX(10px);
}
</style>
