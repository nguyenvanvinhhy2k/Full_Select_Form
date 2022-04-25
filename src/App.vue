<template>
  <div id="app">
    <div class="header">
      <div class="logo">
        <img src="./assets/logoo.png" alt="" />
      </div>
      <div class="menu">
        <ul>
          <li style="font-weight: 900">入社手続き</li>
          <li>ヘルプ</li>
        </ul>
      </div>
    </div>
    <div class="section">
      <div class="content-wrap">
        <div class="content-title">
          <div class="link">
            <img class="img" src="./assets/ArrowLeft.svg" alt="" />
            <h3>雇用契約に戻る</h3>
          </div>
          <h2 style="margin: 0 12px; font-size: 28px">雇用契約について</h2>
        </div>
        <div class="icon-steps">
          <StepsIcon></StepsIcon>
        </div>
        <div class="date">
          <img
            class="icon-date"
            style="margin-bottom: 15px"
            src="./assets/date.png"
            alt=""
          />
        </div>
      </div>
    </div>
    <div class="notice">
      <div class="notice-header">
        <div class="icon">
          <img
            style="width: 25px; margin-right: 10px"
            src="./assets/frame.svg"
            alt=""
          />
        </div>
        <div class="notice-title">
          <h3>ご確認ください</h3>
        </div>
      </div>

      <div class="notice-content">
        <h3 style="font-weight: 400; margin: 0">
          表示されている内容を確認いただき、認識に相違が無ければ同意するにチェックをしてください。
        </h3>
      </div>
    </div>
    <div class="step-1">
      <FirstStep></FirstStep>
    </div>
  </div>
</template>

<script>
import FirstStep from "./components/firstStep.vue";
import StepsIcon from "./components/StepsIcon.vue";
export default {
  name: "App",
  components: { StepsIcon, FirstStep },
  data() {
    return {};
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 0;
  padding: 0;
}
.notice {
  width: 500px;
  margin: 0 auto;
  background-color: #dcdcdc;
}

.notice-header {
  display: flex;
  align-items: center;
}
.icon-steps {
  padding: 20px 0;
}
.section {
  width: 100%;
}
.content-wrap {
  position: relative;
  max-width: 500px;
  margin: 0 auto;
  padding-top: 20px;
}
.icon-date {
  width: 60%;
}
.header {
  width: 1440px;
  height: 64px;
  left: calc(50% - 1440px / 2);
  display: flex;
  align-items: center;
}
ul {
  display: flex;
}
li {
  margin-right: 20px;
  font-size: 20px;
  list-style: none;
}
.img-icon {
  width: 40px;
  height: 40px;
  left: calc(50% - 40px / 2 - 265px);
  top: 168px;
  margin-right: 41px;
  border-radius: 50%;
  background: #b2b1ff;
}
.icon-steps::after {
  content: "";
  width: 23.43rem;
  height: 2px;
  display: block;
  background-color: #dcdcdc;
  position: absolute;
  top: 65.5%;
  left: 8%;
  transform: translateY(-50%);
}
.img {
  width: 30px;
  padding-right: 10px;
}
.notice-content {
  padding: 10px;
}
.logo {
  width: 80px;
}
img {
  width: 63px;

  margin-left: 15px;
}
.link {
  display: flex;
}
</style>
