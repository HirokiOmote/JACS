<template>
  <article>
    <div id="invite" class="container">
      <h2>最新作品建築希望者大募集！</h2>
      <p>現在、2016年住宅設計コンペ「思いやりのある戸建て住宅」にて特別実現採用賞を受賞した作品「棲みかのおすそ分け」を実際に実際に建てて住んでみたい一般の方、また、事業に活かしたい建築、不動産業者様を募集しています。<br>住宅とは基本的には利己的なもの。そんな常識を覆す、周囲の環境にも配慮した「思いやりのある戸建て住宅」をコンセプトとして、実現可能なレベルに最も近い作品として選ばれた「棲みかのおすそ分け」で、豊かな暮らしを体験してみませんか？</p>
      <p class="catch">2016年 JACS住宅設計コンペ「テーマ：思いやりのある戸建て住宅」<br>特別実現採用賞　「棲みかのおすそわけ」</p>
      <p>周囲の環境に対して、時を選ばず、自由に参加できる場をもつこと。<br>
      それが「思いやり」のある建ち方だと考える。<br>
      住宅のすみを周囲にひらくことにより、街の棲み家をつくる。<br>
      街の棲み家の延長に、住人のふるまいが表出することで、他人が住人活動の場に参加するきっかけをあたえる。<br>
      1枚の壁に様々な棲み家が連鎖することで、居場所のグラデーションを生む。<br>
      1人になれる「孤独の場」と、複数で集まれる「参加の場」を選択できる、思いやりのある場をつくりたい。</p>
      <div><img src="../assets/images/img_invite.jpg" alt=""></div>
      <ul>
        <li><a href="./static/images/2016concept.pdf">コンセプトPDF</a></li>
        <li><a href="./static/images/2016zu.pdf">解説図面PDF</a></li>
      </ul>
      <p>実際に建築する建物に関しましては、作品と全く同じものということではなく、ステーツの建築ノウハウを活かし、お客様のライフスタイルを考えながら、実際に生活を営むにあたり快適に過ごせるレベルにブラッシュアップしたものになりますので、ご安心ください。<br>
      コンセプトにご共感いただけた方、ご相談お見積等をご希望の方は、以下よりお気軽にお問い合わせください。</p>
      <a class="contactBtn" href="https://www.states.co.jp/contact/">作品実現についてお問い合わせ</a>
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
    &.catch {
      font: {
        size: 1.8rem;
        weight: 600;
      }
      line-height: 1.3;
      @include media( sm ) {
        font-size: 2.1em;
      }
      @include media( sm ) {
        font-size: 2.4em;
      }
    }
  }

  ul {
    max-width: 100%;
    padding: 0;
    text-align: center;
    li {
      margin-top: 1em;
      a {
        @include btn;
      }
    }
    @include media( md ) {
      display: flex;
      justify-content: space-between;
      li {
        width: 48%;
      }
    }
  }

  .contactBtn {
    @include btn( #deaa2c, #aa7d11 );
    margin-top: 4rem;
  }
</style>
