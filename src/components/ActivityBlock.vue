<template>
  <article>
    <div class="container">
      <h2>JACSの活動内容</h2>
      <p class="catch">全10回に渡る<br class="visible-xs">「住宅設計コンペ」を開催</p>
      <p>JACSでは過去１０年間に渡り、毎年１回学生たちが参加する「住宅設計コンペ」を開催して参りました。<br>
      各回ごとに決められたテーマに沿い、学生たちが常識にとらわれない斬新で豊かな発想の「住宅」を発案しながら<br class="hidden-sm">
      競い合うことで、より洗練されたアイデアを養い全体的なレベルアップを図るための発展と交流の場となりました。</p>
    </div>
  </article>
</template>

<script>
export default {
  name: 'ActivityBlock',
};
</script>

<style lang="scss" scoped>
  @import "../assets/stylesheets/_mixin";

  article {
    margin: 60px 0;
    &::after {
      content: "";
      display: block;
      width: 100%;
      height: 170px;
      margin-top: 2.5rem;
      background: #ededed url("../assets/images/bg_activity.jpg") left 50% bottom 0 no-repeat;
      background-size: cover;
      @include media( sm ) {
        height: 250px;
      }
      @include media( md ) {
        height: 350px;
      }
    }
  }
  .container {
    @include container;
  }
  h2 {
    @include title;
  }
  p {
    text-align: left;
    @include media( sm ) {
      text-align: center;
    }
  }
  .catch {
    @include catch;
    text-align: center;
  }
</style>
