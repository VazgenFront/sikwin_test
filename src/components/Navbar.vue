<template>
  <div>
    <div class="header width80pr">
      <div class="header-left">
        <div class="social-sites">
          <img src="@/assets/youtube.png" alt="" />
          <img src="@/assets/instagram.png" alt="" />
          <img src="@/assets/facebook.png" alt="" />
          <img src="@/assets/telegram.png" alt="" />
        </div>
        <div class="logo">
          <img src="@/assets/logo.png" alt="" />
        </div>
      </div>

      <div class="header-right">
        <div class="login-register">
          <button class="login">Login</button>
          <button class="register">Sign-up</button>
        </div>
        <div class="select-lang">
          <img src="@/assets/USA-flag.png" alt="" />
          <span>English</span>
          <img src="@/assets/toggle-arrow.png" alt="" />
        </div>
      </div>
    </div>

    <nav>
      <ul class="navbar">
        <a href="#" class="app-download">APP DOWNLOAD</a>
        <li class="active">
          <img src="@/assets/home-logo.png" alt="" />
          <a href="#">HOME</a>
        </li>
        <li class="live-casino">
          <img src="@/assets/live-casino.png" class="icon" alt="" />
          <a href="#">LIVECASINO</a>
          <div class="nav-info">
            <div class="hidden-menu">
              <div class="div-img">
                <img src="@/assets/QR.jpg" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img1.png" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img2.png" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img3.png" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img4.png" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img5.png" alt="" />
              </div>
            </div>
          </div>
        </li>
        <li class="sport">
          <img src="@/assets/ball.png" class="icon" alt="" />
          <a href="#">SPORT</a>
          <div class="nav-info">
            <div class="hidden-menu hidden-menu2">
              <div class="div-img">
                <img src="@/assets/img2.1.png" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img2.2.png" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img2.3.jpg" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img2.4.jpg" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img2.5.png" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img2.3.jpg" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img2.6.png" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img2.7.png" alt="" />
              </div>
            </div>
          </div>
        </li>
        <li class="lottery">
          <img src="@/assets/lottery-logo.png" class="icon" alt="" />
          <a href="#">LOTTERY</a>
          <div class="nav-info">
            <div class="hidden-menu">
              <div class="div-img">
                <img src="@/assets/img3.1.png" alt="" />
              </div>
              <div class="div-img">
                <img src="@/assets/img3.2.png" alt="" />
              </div>
            </div>
          </div>
        </li>

        <li class="patti">
          <img src="@/assets/teen-patti.png" class="icon" alt="" />
          <a href="#">TEEN PATTI</a>
        </li>
        <li class="cardgame">
          <img src="@/assets/cardgame.png" class="icon" alt="" />
          <a href="#">CARDGAME</a>
        </li>
        <li class="slot">
          <img src="@/assets/slot.png" class="icon" alt="" />
          <a href="#">SLOT</a>
        </li>
        <li class="prom">
          <img src="@/assets/prom.png" class="icon" alt="" />
          <a href="#">PROMOTION</a>
        </li>
        <li class="customer">
          <img src="@/assets/customer.png" class="icon" alt="" />
          <a href="#">CUSTOMER</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
  export default {
    name: "navbar-item",
  };
</script>

<style scoped>
  header {
    background: #000;
  }

  .header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 15px 20px;
  }
  .header-left {
    display: flex;
    align-items: center;
  }

  .header-right {
    display: flex;
    align-items: center;
  }

  .social-sites img {
    width: 30px;
    margin-right: 15px;
    cursor: pointer;
  }

  .logo {
    max-width: 150px;
  }
  .logo img {
    width: 100%;
    cursor: pointer;
  }

  .login,
  .register {
    width: 95px;
    height: 35px;
    font-size: 16px;
    border-radius: 7px;
    color: #fff;
    text-align: center;
    margin-right: 20px;
    cursor: pointer;
  }
  .login {
    background: #ff0000;
    border: 1px solid #ff0000;
  }
  .register {
    background: #efb158;
    border: 1px solid #efb158;
  }

  .select-lang {
    display: flex;
    align-items: center;
    color: #fff;
    font-size: 14px;
    cursor: pointer;
  }
  .select-lang span {
    margin: 0 10px;
  }

  nav {
    border-top: 2px solid #efb158;
  }

  .navbar {
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
  }
  .navbar a {
    color: #e2e2e2;
    font-size: 16px;
  }
  .navbar li {
    width: 130px;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .app-download {
    width: 166px;
    height: 51px;
    font-size: 16px;
    color: rgb(226, 226, 226);
    white-space: nowrap;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    background: #3e3d3d;
  }

  .active {
    color: #fff;
    background: #efb158;
  }
  .active img {
    margin-right: 5px;
  }

  .active:hover {
    background: #3e3d3d;
  }

  .nav-info {
    width: 100%;
    height: 0;
    display: flex;
    position: absolute;
    left: 0;
    top: 50px;
    background: url(@/assets/hidden-bg.png);
    overflow: hidden;
    transition: 0.3s;
    z-index: 9;
  }

  .nav-info img {
    width: 160px;
  }

  .hidden-menu {
    height: 250px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .hidden-menu2 {
    margin-left: -100px;
  }

  .div-img {
    width: 220px;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .div-img:hover {
    background: #ffffff58;
  }

  .live-casino:hover,
  .sport:hover,
  .lottery:hover,
  .patti:hover,
  .cardgame:hover,
  .slot:hover,
  .prom:hover,
  .customer:hover {
    background: #3e3d3d;
  }
  .live-casino:hover .icon,
  .sport:hover .icon,
  .lottery:hover .icon,
  .patti:hover .icon,
  .cardgame:hover .icon,
  .slot:hover .icon,
  .prom:hover .icon,
  .customer:hover .icon {
    display: block;
    background: #3e3d3d;
  }
  .live-casino:hover .nav-info,
  .sport:hover .nav-info,
  .lottery:hover .nav-info {
    height: 250px;
  }

  .icon {
    display: none;
    margin-right: 5px;
    cursor: pointer;
  }

  li {
    list-style: none;
  }
</style>
