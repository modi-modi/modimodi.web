<template>
  <div id="app">
    <header>
      <div class="logo"></div>
      <nav>
        <router-link to="/">로그인</router-link> |
        <router-link to="/about">회원가입</router-link> |
        <router-link to="/about">주문조회</router-link> |
        <router-link to="/about">장바구니</router-link>
      </nav>
    </header>
    <aside>
      <ul>
        <li>
          소개
        </li>
        <li>
          카탈로그
        </li>
        <li>
          상품
        </li>
        <li>
          기타
        </li>
      </ul>
    </aside>
    <main>
      <router-link></router-link>
    </main>
    <footer></footer>
  </div>
</template>

<style lang="scss">
* {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
}
aside {
  width: 130px;
  margin-left: 0;
  float: left;
}
nav {
  padding: 30px;
  a {
    text-align: right;
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
.logo {
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
</style>
