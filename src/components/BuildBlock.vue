<template>
  <article>
    <h2>「思いやりのある戸建て住宅」<br class="visible-xs">建築希望者　大募集！</h2>
    <p>現在、当コンソーシアムが開催する第10回住宅設計コンペ「テーマ：思いやりのある戸建て住宅」にて、<br class="hidden-sm">
    実現可能なレベルに最も近い作品として選ばれた「棲みかのおすそ分け」を、実際に建てて住んでみたい方、<br class="hidden-sm">
    また、事業に活かしたい建築、不動産業者様を募集しています。</p>
    <div><img src="../assets/images/img_build.jpg" alt=""></div>
    <p class="Note">作品のコンセプト等詳細に関しましては、<br class="visible-xs">以下よりご覧ください。</p>
    <a href="">作品詳細を見る</a>
  </article>
</template>

<script>
export default {
  name: 'BuildBlock',
};
</script>

<style lang="scss" scoped>
@import "../assets/stylesheets/_mixin";

article {
  @include container;
  margin: {
    top: 40px;
    bottom: 40px;
  }
  background-color: #fff;
  @include media( md ) {
    margin-top: -90px;
    padding-top: 25px;
  }
}

h2 {
  @include catch;
}

p {
  text-align: left;
  margin-top: 2.5em;
  &.Note {
    font-size: 1.5rem;
    font-weight: 600;
    line-height: 1.5;
    text-align: center;
  }
  @include media( sm ) {
    text-align: center;
    &.Note {
      font-size: 2.1rem;
    }
  }
}

a {
  @include btn;
}

</style>
