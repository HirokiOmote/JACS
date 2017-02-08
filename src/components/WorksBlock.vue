<template>
  <article>
    <h2>建築実現作品</h2>
    <p>応募作品のデザインとコンセプトを一般化、ブラッシュアップし実際に建築。<br>
    その斬新で豊かな発想の「住宅」を ”カタチ” にしました。<br>
    <br>
    2007～2008年最優秀作品は、現在も新潟市秋葉区にてモデルハウスとして公開中。<br>
    以下に、その作品と実例を紹介いたします。</p>
    <figure>
      <figcaption>CAR × ROOF</figcaption>
      <p>一階に大きな庭のような車庫を設けてその間に個室をばら撒きました。</p>
      <ul>
        <li><img src="../assets/images/img_works001.jpg" alt=""></li>
        <li><img src="../assets/images/img_works002.jpg" alt=""></li>
        <li><img src="../assets/images/img_works003.jpg" alt=""></li>
        <li><img src="../assets/images/img_works004.jpg" alt=""></li>
        <li><img src="../assets/images/img_works005.jpg" alt=""></li>
      </ul>
    </figure>
    <figure>
      <figcaption>した庭の家</figcaption>
      <p>一階に大きな庭のような車庫を設けてその間に個室をばら撒きました。</p>
      <ul>
        <li><img src="../assets/images/img_works006.jpg" alt=""></li>
        <li><img src="../assets/images/img_works007.jpg" alt=""></li>
        <li><img src="../assets/images/img_works008.jpg" alt=""></li>
        <li><img src="../assets/images/img_works009.jpg" alt=""></li>
        <li><img src="../assets/images/img_works010.jpg" alt=""></li>
      </ul>
    </figure>
  </article>
</template>

<script>
export default {
  name: 'WorksBlock',
};
</script>

<style lang="scss" scoped>
  @import "../assets/stylesheets/_mixin";

  article {
    @include container;
    margin: {
      top: 60px;
      bottom: 60px;
    }
  }

  h2 {
    @include title;
  }

  figure {
    margin: 4rem 0 0 0 ;
  }

  figcaption {
    font: {
      size: 1.6rem;
      weight: 600;
    }
    @include media( sm ) {
      font: {
        size: 2.1rem;
      }
    }
  }

  ul {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    margin: 1rem -7.5px;
    padding: 0;
    @include media( sm ) {
      justify-content: space-between;
    }
  }

  li {
    position: relative;
    z-index: 1;
    width: calc( 100% / 2 - 15px );
    line-height: 0;
    margin: 7.5px;
    &:first-child {
      width: 100%;
      img {
        width: auto;
        box-sizing: border-box;
        border: 8px solid #e4e4e4;
      }
      &::after {
        content: "▼";
        display: block;
        color: #e4e4e4;
        font-size: 30px;
        width: 20px;
        position: absolute;
        right: calc( 50% - 6px );
        bottom: -3px;
        z-index: 2;
      }
    }
    img {
      position: relative;
      z-index: 10;
      width: 100%;
    }
    @include media( sm ) {
      width: calc( 100% / 5 - 15px );
      margin: 7.5px;
      &:first-child {
        width: calc( 100% / 5 - 15px );
        &::after {
          right: -10px;
          top: 51%;
          bottom: auto;
          transform: rotate(270deg);
        }
      }
    }
  }
</style>
