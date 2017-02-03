<template>
  <article>
    <h2>住宅設計コンペ実例集</h2>
    <p>全10回全ての住宅設計コンペの優秀作品をご紹介いたします。<br class="hidden-sm">
    全国より集結した若き建築家による力作をご覧ください。</p>
    <ul class="exampleList">
      <li><img src="../assets/images/img_example001.jpg" alt=""></li>
      <li><img src="../assets/images/img_example002.jpg" alt=""></li>
      <li><img src="../assets/images/img_example003.jpg" alt=""></li>
      <li><img src="../assets/images/img_example004.jpg" alt=""></li>
      <li><img src="../assets/images/img_example005.jpg" alt=""></li>
      <li><img src="../assets/images/img_example006.jpg" alt=""></li>
      <li><img src="../assets/images/img_example007.jpg" alt=""></li>
      <li><img src="../assets/images/img_example008.jpg" alt=""></li>
      <li><img src="../assets/images/img_example009.jpg" alt=""></li>
      <li><img src="../assets/images/img_example010.jpg" alt=""></li>
    </ul>
    <aside>
      <h3>その他受賞作品に関してましては、<br class="visible-xs">以下PDFファイルをご覧ください。</h3>
      <ul class="otherList">
        <li><a href="#" target="_blanck">●●●●●●●●●●●●作品PDF</a></li>
        <li><a href="#" target="_blanck">●●●●●●●●●●●●作品PDF</a></li>
        <li><a href="#" target="_blanck">●●●●●●●●●●●●作品PDF</a></li>
        <li><a href="#" target="_blanck">●●●●●●●●●●●●作品PDF</a></li>
        <li><a href="#" target="_blanck">●●●●●●●●●●●●作品PDF</a></li>
        <li><a href="#" target="_blanck">●●●●●●●●●●●●作品PDF</a></li>
      </ul>
    </aside>
  </article>
</template>

<script>
export default {
  name: 'ExampleBlock',
};
</script>

<style lang="scss" scoped>
  @import "../assets/stylesheets/_mixin";

  article {
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

  .exampleList {
    display: flex;
    flex-wrap: wrap;
    width: calc( 100% + 15px );
    margin: 2.5rem -7.5px;
    padding: 0;
    li {
      width: calc( 100% / 2 - 15px );
      margin: 7.5px;
      line-height: 0;
      text-align: center;
    }
    @include media( sm ) {
      margin: 2.5rem auto;
      width: 100%;
      li {
        width: calc( 100% / 5 - 15px );
      }
    }
  }

  aside {
    margin: 60px -15px 0;
    padding: 25px;
    background-color: #e4e4e4;
    @include media( sm ) {
      text-align: left;
    }
    h3 {
      display: inline-flex;
      align-items: center;
      font {
        size: 1.4rem;
        weight: normal;
      }
      line-height: 1.3;
      &:before {
        content: url("../assets/images/img_iconPDF.png");
        margin-right: .5em;
      }
      @include media( sm ) {
        font-size: 1.5rem;
      }
      @include media( md ) {
        font-size: 1.6rem;
      }
    }
  }

  .otherList {
    padding: 0;
    li {
      margin: 1em 0;
      font-size: 1.4rem;
    }
    @include media( sm ) {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      li {
        padding: 0 1.9em;
        font-size: 1.6rem;
      }
    }
  }
</style>
