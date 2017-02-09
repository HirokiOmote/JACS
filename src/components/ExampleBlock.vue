<template>
  <article>
    <h2>住宅設計コンペ実例集</h2>
    <p>全10回全ての住宅設計コンペの優秀作品をご紹介いたします。<br class="hidden-sm">
    全国より集結した若き建築家による力作をご覧ください。</p>
    <ul class="exampleList">
      <li>
        <figure>
          <h1>2007</h1>
          <img src="../assets/images/img_example001.jpg" alt="">
          <figcaption>
            <span>テーマ</span><br>
            ｢未来」<br>
            <span>コンセプト</span><br>
            ｢CAR×ROOF」
          </figcaption>
        </figure>
      </li>
      <li>
        <figure>
          <h1>2008</h1>
          <img src="../assets/images/img_example002.jpg" alt="">
          <figcaption>
            <span>テーマ</span><br>
            ｢環境」<br>
            <span>コンセプト</span><br>
            ｢した庭の家」
          </figcaption>
        </figure>
      </li>
      <li>
        <figure>
          <h1>2009</h1>
          <img src="../assets/images/img_example003.jpg" alt="">
          <figcaption>
            <span>テーマ</span><br>
            ｢50年デザイン住宅」<br>
            <span>コンセプト</span><br>
            ｢活動のカベと<br>
            　　　小さなコシツ」
          </figcaption>
        </figure>
      </li>
      <li>
        <figure>
          <h1>2010</h1>
          <img src="../assets/images/img_example004.jpg" alt="">
          <figcaption>
            <span>テーマ</span><br>
            ｢住まいの原点を再考する」<br>
            <span>コンセプト</span><br>
            ｢豊かな家」
          </figcaption>
        </figure>
      </li>
      <li>
        <figure>
          <h1>2011</h1>
          <img src="../assets/images/img_example005.jpg" alt="">
          <figcaption>
            <span>テーマ</span><br>
            ｢環境住宅 光と風」<br>
            <span>コンセプト</span><br>
            ｢からまりの家」
          </figcaption>
        </figure>
      </li>
      <li>
        <figure>
          <h1>2012</h1>
          <img src="../assets/images/img_example006.jpg" alt="">
          <figcaption>
            <span>テーマ</span><br>
            ｢自分の家」<br>
            <span>コンセプト</span><br>
            ｢渦巻く長廊家」
          </figcaption>
        </figure>
      </li>
      <li>
        <figure>
          <h1>2013</h1>
          <img src="../assets/images/img_example007.jpg" alt="">
          <figcaption>
            <span>テーマ</span><br>
            ｢郊外住宅の新定義」<br>
            <span>コンセプト</span><br>
            ｢kiosk×house」
          </figcaption>
        </figure>
      </li>
      <li>
        <figure>
          <h1>2014</h1>
          <img src="../assets/images/img_example008.jpg" alt="">
          <figcaption>
            <span>テーマ</span><br>
            ｢大きな土地の１人暮らしの家」<br>
            <span>コンセプト</span><br>
            ｢歓びの三角屋根」<br>
          </figcaption>
        </figure>
      </li>
      <li>
        <figure>
          <h1>2015</h1>
          <img src="../assets/images/img_example009.jpg" alt="">
          <figcaption>
            <span>テーマ</span><br>
            ｢母の家」<br>
            <span>コンセプト</span><br>
            ｢ひとりの場所と<br>
            　　　みんなの場所」
          </figcaption>
        </figure>
      </li>
      <li>
        <figure>
          <h1>2016</h1>
          <img src="../assets/images/img_example010.jpg" alt="">
          <figcaption>
            <span>テーマ</span><br>
            ｢思いやりのある
            　　　　戸建て住宅」<br>
            <span>コンセプト</span><br>
            ｢暮らしが息づく
            　　　　　　住まい」
          </figcaption>
        </figure>
      </li>
    </ul>
    <aside>
      <h3>その他受賞作品に関してましては、<br class="visible-xs">以下PDFファイルをご覧ください。</h3>
      <ul class="otherList">
        <li><a href="./static/images/2007jacs.pdf" target="_blank">2007作品PDF</a></li>
        <li><a href="./static/images/2008jacs.pdf" target="_blank">2008作品PDF</a></li>
        <li><a href="./static/images/2009jacs.pdf" target="_blank">2009作品PDF</a></li>
        <li><a href="./static/images/2010jacs.pdf" target="_blank">2010作品PDF</a></li>
        <li><a href="./static/images/2011jacs.pdf" target="_blank">2011作品PDF</a></li>
        <li><a href="./static/images/2012jacs.pdf" target="_blank">2012作品PDF</a></li>
        <li><a href="./static/images/2013jacs.pdf" target="_blank">2013作品PDF</a></li>
        <li>2014作品PDF</li>
        <li><a href="./static/images/2015jacs.pdf" target="_blank">2015作品PDF</a></li>
        <li><a href="./static/images/2016jacs.pdf" target="_blank">2016作品PDF</a></li>
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
      font-size: 1.2rem;
      line-height: 1.5;
      text-align: left;
    }
    figure {
      margin: 0;
    }
    h1 {
      font-size: inherit;
    }
    span {
      font-size: .75em;
    }
    @include media( sm ) {
      margin: 2.5rem auto;
      width: 100%;
      li {
        font-size: 1.4rem;
        width: calc( 100% / 5 - 15px );
      }
    }
    @include media( md ) {
      font-size: 1.6rem;
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
