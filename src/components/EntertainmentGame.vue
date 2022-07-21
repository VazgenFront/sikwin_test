<template>
  <section class="section3">
    <div class="sec3-div width80pr">
      <div class="girl">
        <img src="@/assets/girl.png" alt="" />
      </div>
      <div class="casino">
        <div
          v-for="ent in entertainments"
          :class="ent.class"
          :key="ent.class + ent + image"
        >
          <div v-if="ent.image" class="casino-logo">
            <img :src="ent.image" :alt="ent.img" />
          </div>
          <div class="casino-txt">
            <p v-if="ent.upText">{{ent.upText}}</p>
            <span v-if="ent.downText">{{ent.downText}}</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "EntertainmentGame-item",

  data: () => ({
    entertainments: [
      {
        class: "casino-item bg-color",
        image: require("@/assets/ae-casino.png"),
        upText: "AE LIVE",
        downText: "Live Casino",
      },
      {
        class: "casino-item",
        image: require("@/assets/pp-live.png"),
        upText: "PP LIVE",
        downText: "Live Casino",
      },
      {
        class: "casino-item bg-color",
        image: "",
        upText: "VIVO LIVE",
        downText: "",
      },
      { class: "casino-item ", image: "", upText: "PT LIVE", downText: "" },
      {
        class: "casino-item bg-color",
        image: require("@/assets/evolution.png"),
        upText: "EVO LIVE",
        downText: "Live Casino",
      },
      {
        class: "casino-item ",
        image: require("@/assets/e-zugi.png"),
        upText: "EZ LIVE",
        downText: "Live Casino",
      },
    ],
  }),
};
</script>

<style scoped>
.section3 {
  background: url(@/assets/background-sec3.png);
  height: 572px;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  background-color: #000c;
}
.sec3-div {
  display: flex;
}

.girl {
  width: 319px;
}
.girl img {
  transition: 1s;
}
.girl img:hover {
  transform: translateX(10px);
}
.casino {
  display: flex;
  flex-wrap: wrap;
}
.casino-item {
  width: 290px;
  height: 290px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}

.casino-txt {
  color: #acacac;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.casino-txt p {
  font-size: 40px;
}
.casino-txt span {
  font-size: 24px;
}

.bg-color {
  background: #ffffff21;
}
.casino-item:hover {
  background: transparent;
  border: 2px solid #ebc86d;
}
</style>
