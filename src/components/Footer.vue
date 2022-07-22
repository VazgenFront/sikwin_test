<template>
  <footer>
    <div class="footer-btn width80pr">
      <p>About us</p>
      <p>Contact us</p>
      <p>Partnership</p>
      <p>Help with deposits and withdrawals</p>
      <p>Q&A</p>
    </div>

    <div class="footer-img width80pr"></div>

    <div class="copyright">
      <p>Copyright @ Sikwin Reserved</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: "footer-item",
};
</script>

<style>
footer {
  padding: 30px 0;
}

.footer-btn {
  color: #bcbcbc;
  display: flex;
  justify-content: center;
  margin-bottom: 30px;
}

.footer-btn p {
  font-size: 16px;
  padding: 0 34px;
  border-right: 1px solid #b4b5b7;
  cursor: pointer;
  display: flex;
  align-items: center;
}
.footer-btn p:last-child {
  border: none;
}
.footer-img {
  background: url(@/assets/foot_bg.a236272b.png) no-repeat;
  height: 50px;
}
.copyright {
  color: #7b7b7b;
  text-align: center;
  margin-top: 25px;
}
</style>
