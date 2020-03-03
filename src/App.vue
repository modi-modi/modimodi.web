<template>
  <div id="app">
    <header>
      <nav>
        <router-link to="/">로그인</router-link> |
        <router-link to="/about">회원가입</router-link> |
        <router-link to="/about">주문조회</router-link> |
        <router-link to="/about">장바구니</router-link>
      </nav>
    </header>
    <aside>
      <div class="logo">
        modimodi
      </div>
      <ul class="aside__menu">
        <li>
          소개
        </li>
        <li>
          카탈로그
        </li>
      </ul>
    </aside>
    <main>
      <router-view></router-view>
    </main>
    <footer></footer>
  </div>
</template>

<style lang="scss">

@font-face {
  font-family: 'Quesat Black';
  src: url('./assets/fonts/Quesat/Quesat Black Demo.otf') format('opentype');
}
@font-face {
  font-family: 'Quesat Black Italic';
  src: url('./assets/fonts/Quesat/Quesat Black Italic Demo.otf') format('opentype');
}
@font-face {
  font-family: 'Quesat Bold';
  src: url('./assets/fonts/Quesat/Quesat Bold Demo.otf') format('opentype');
}
@font-face {
  font-family: 'Quesat Bold Italic';
  src: url('./assets/fonts/Quesat/Quesat Bold Italic Demo.otf') format('opentype');
}
@font-face {
  font-family: 'Quesat Demi Bold';
  src: url('./assets/fonts/Quesat/Quesat Demi Bold Demo.otf') format('opentype');
}
@font-face {
  font-family: 'Quesat Demi Bold Italic';
  src: url('./assets/fonts/Quesat/Quesat Demi Bold Italic Demo.otf') format('opentype');
}
@font-face {
  font-family: 'Quesat Italic';
  src: url('./assets/fonts/Quesat/Quesat Italic Demo.otf') format('opentype');
}
@font-face {
  font-family: 'Quesat Light';
  src: url('./assets/fonts/Quesat/Quesat Light Demo.otf') format('opentype');
}
@font-face {
  font-family: 'Quesat Light Italic';
  src: url('./assets/fonts/Quesat/Quesat Light Italic Demo.otf') format('opentype');
}
@font-face {
  font-family: 'Quesat Regular';
  src: url('./assets/fonts/Quesat/Quesat Regular Demo.otf') format('opentype');
}

* {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
}
#app {
    // color: ${theme.text.default};
    width: 100%;
    height: 100%;
    margin-top: 0px;
    margin-right: 201px;
    position: relative;
    top: 10px;
    padding-top: 0;
    transition: margin-right 0.3s ease-out;
    -webkit-transition: margin-right 0.3s ease-out;
}
#app:before {
    content: '';
    position: fixed;
    top: 0;
    bottom: 0;
    z-index: -2;
    left: 0;
    right: 0;
    background-image: -moz-radial-gradient(circle farthest-corner, #fec1c0 0%, #f7dedd 70%);
    background-image: -o-radial-gradient(circle farthest-corner, #fec1c0 0%, #f7dedd 70%);
    background-image: -webkit-radial-gradient(circle farthest-corner, #fec1c0 0%, #f7dedd 70%);
    background-image: radial-gradient(circle farthest-corner at top, #fec1c0 0%, #f7dedd 70%);
    background-position: 50%, 50%;
}
aside {
  width: 130px;
  margin-left: 0;
  float: left;
}
nav {
  text-align: right;
  // padding: 30px;
  padding-right: 20px;
  a {
    // text-align: right;
    font-size: 0.7rem;
    // font-weight: 600;
    color: #2c3e50;
    text-decoration: none;
    &.router-link-exact-active {
      font-weight: bold;
    }
  }
}
.logo__img {
  padding: 15px;
  position: relative;
  display: inline-block;
  width: 120px;
  height: 120px;
  background-image: url(/img/modimodi.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  border-radius: 50%
}

.logo {
  user-select: none;
  cursor: pointer;
  position: relative;
  width: 100%;
  height: 120px;
  border: 4px solid #fec1c0;
  border-radius: 50%;
  background-color: #f7dedd;
  // border-style: solid;
  // border-image-source: linear-gradient(to bottom, #fff042, #ff5451);
  // border-image: linear-gradient(to right, #fec1c0 20%, #f7dedd 70%);
  // background-image: -moz-radial-gradient(circle at left, #fec1c0 0%, #f7dedd 70%);
  // background-image: -o-radial-gradient(circle at left, #fec1c0 0%, #f7dedd 70%);
  // background-image: -webkit-radial-gradient(circle at left, #fec1c0 0%, #f7dedd 70%);
  // background-image: radial-gradient(circle at left, #fec1c0 0%, #f7dedd 70%);
  background-position: 50%, 50%;
  background-origin: border-box;
  background-clip: content-box, border-box;
  display: flex;
  align-items: center;
  justify-content: center;
  // border-image-slice: 20;
  // padding-top: 40%;
  margin: 2px;
  // margin-left: 10px;
  // padding: 15px;
  color: #04a2ff;
  font-size: 25px;
  font-family: 'Quesat Bold Italic';
}
aside {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
}
.aside__menu {
  font-size: 0.8rem;
  // padding-left: 4px;
}
.aside__menu li{
  padding: 4px;
  list-style: none;
  text-align: left;
}
</style>
