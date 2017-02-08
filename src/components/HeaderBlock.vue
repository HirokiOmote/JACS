<template>
  <header>
    <div class="topBar">
      <div class="Logo"><img src="../assets/images/img_logo.png" alt="株式会社ステーツ"></div>
      <div class="Tel"><img src="../assets/images/img_tel.png" alt="0120-666-940"></div>
    </div>
    <div class="bgContent">
        <h1><img src="../assets/images/img_header.png" alt=""></h1>
        <h2>ステーツは建築学生を応援するコンソーシアムを運営しています</h2>
        <p>JACS（全日本学生建築コンソーシアム）は、建築を学ぶ学生の皆様のレベルアップと交流の場を<br class="hidden-sm">
        サポートするために設立された、学生による学生のためのコンソーシアムです。<br><br>
        JACSでは住宅業界全体の活性化と発展、そして未来の住宅の模索などに貢献し、<br class="hidden-sm">
        一般社会と学生の思考や技術の交流を高めることを目的としています。</p>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderBlock',
};
</script>

<style lang="scss" scoped>
@import "../assets/stylesheets/_mixin";

.topBar {
  @include container;
  padding: {
    top: 20px;
    bottom: 20px;
  }
  @include media( sm ) {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}

h2 {
  margin-top: 30px;
  font-size: 2.2em;
}

.Tel {
  margin-top: 20px;
  img {
    max-width: 150px;
  }
  @include media( sm ) {
    margin-top: 0;
  }
  @include media( md ) {
    img {
      max-width: none;
    }
  }
}


.bgContent {
  padding: 80px 15px;
  background: url("../assets/images/bg_header.jpg") center bottom -165px no-repeat;
  @include media( sm ) {
    padding: 30px 15px 250px;
    background-position: center bottom -55px;
  }
  @include media( lg ) {
    background-size: cover;
  }
  p {
    text-align: left;
    margin-top: 20px;
    @include media( sm ) {
      text-align: center;
    }
  }
}
</style>
