<template>
  <article>
    <div class="container">
      <h2>最新作品建築希望者大募集！</h2>
      <p>現在、2016年住宅設計コンペ「思いやりのある戸建て住宅」にて特別実現採用賞を受賞した作品「棲みかのおすそ分け」を実際に実際に建てて住んでみたい一般の方、また、事業に活かしたい建築、不動産業者様を募集しています。<br>住宅とは基本的には利己的なもの。そんな常識を覆す、周囲の環境にも配慮した「思いやりのある戸建て住宅」をコンセプトとして、実現可能なレベルに最も近い作品として選ばれた「棲みかのおすそ分け」で、豊かな暮らしを体験してみませんか？</p>
      <div><img src="../assets/images/img_invite.jpg" alt=""></div>
      <p>実際に建築する建物に関しましては、作品と全く同じものということではなく、ステーツの建築ノウハウを活かし、お客様のライフスタイルを考えながら、実際に生活を営むにあたり快適に過ごせるレベルにブラッシュアップしたものになりますので、ご安心ください。<br>
      コンセプトにご共感いただけた方、ご相談お見積等をご希望の方は、以下よりお気軽にお問い合わせください。</p>
      <a href="">作品実現についてお問い合わせ</a>
    </div>
  </article>
</template>

<script>
export default {
  name: 'InviteBlock',
};
</script>

<style lang="scss" scoped>
  @import "../assets/stylesheets/_mixin";

  article {
    padding: 60px 0;
    background-color: #ededed;
  }

  .container {
    @include container;
  }

  h2 {
    @include title;
  }

  p {
    text-align: left;
  }

  a {
    @include btn( #deaa2c, #aa7d11 );
    margin-top: 4rem;
  }
</style>
