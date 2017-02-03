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
      <ul>
        <li><img src="../assets/images/img_works001.jpg" alt=""></li>
        <li><img src="../assets/images/img_works002.jpg" alt=""></li>
        <li><img src="../assets/images/img_works003.jpg" alt=""></li>
        <li><img src="../assets/images/img_works004.jpg" alt=""></li>
      </ul>
    </figure>
    <figure>
      <figcaption>AROSMH</figcaption>
      <ul>
        <li><img src="../assets/images/img_works005.jpg" alt=""></li>
        <li><img src="../assets/images/img_works006.jpg" alt=""></li>
        <li><img src="../assets/images/img_works007.jpg" alt=""></li>
        <li><img src="../assets/images/img_works008.jpg" alt=""></li>
      </ul>
    </figure>
    <a href="#">施工事例のリンク</a>
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
    margin: 1rem -7.5px;
    padding: 0;
    @include media( sm ) {
      justify-content: space-between;
    }
  }

  li {
    line-height: 0;
    width: calc( 100% / 2 - 15px );
    margin: 7.5px;
    img {
      width: 100%;
    }
    @include media( sm ) {
      margin: 12.5px;
      width: calc( 100% / 4 - 25px );
    }
  }

  a {
    @include btn;
  }
</style>
