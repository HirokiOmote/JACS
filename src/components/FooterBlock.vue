<template>
  <footer>
    <div class="container">
      <p class="Logo"><img src="../assets/images/img_footerlogo.png" alt="株式会社ステーツ"></p>
      <p><small>Copyright &copy; STATES CO.,LTD All Rights Reserved.</small></p>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterBlock',
};
</script>

<style lang="scss" scoped>
@import "../assets/stylesheets/_mixin";

footer {
  padding: 13px 0;
  background-color: #f9f9f9;
}
.Logo {
  display: none;
  @include media( sm ) {
    display: block;
  }
}
.container {
  @include container;
  @include media( sm ) {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}
</style>
