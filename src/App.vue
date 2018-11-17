<template>
  <div id="app">
    <router-view></router-view>

    <footer>
      <p class="footer-ctx margin-sides">沪ICP备18024906号-1 Copyright © 2018 上海洋檀棱桃文化传播有限公司</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  overflow-x: hidden;
  font-family: 'PingFang HK', 'Hiragino Sans GB', '冬青黑体', "Microsoft Yahei", "微软雅黑", 'STXihei', "华文细黑", 'SimHei', '黑体', 'Hei Ti', 'Helvetica neue', Helvetica, sans-serif
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

* {
  color: #000;
}

/* Multi-use classes */
.display-f {
  display: flex;
}
.display-n {
  display: none;
}

.d-flex-center {
  display: flex;
  justify-content: center;
}
.container {
  max-width: 1000px;
  width: 100%;
}
.margin-sides {
  margin: 0 25px;
}
.shadow {
  box-shadow: 25px 25px 25px rgba(0, 0, 0, 0.1);
}
.p-text {
  font-size: 1rem;
  line-height: 1.5rem
}
.mb-0 {
  margin-bottom: 0  !important;
}
/**/

footer {
  height: 50px;
  background: #fccd0f;
  display: flex;
  justify-content: center;
  align-items: center;
}
  .footer-ctx {
    color: #fefbef;
    font-size: 12px;
  }

@media (max-width: 550px){
  html {
    font-size: 12px;
  }
  .shadow {
    box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.1);
  }
}

</style>
