<template>
  <section>
    <h2>JACS協賛メーカー様一覧</h2>
    <ul>
      <li><a href="#"><img src="../assets/images/img_logo.png" alt=""></a></li>
      <li><a href="#"><img src="../assets/images/img_logo.png" alt=""></a></li>
      <li><a href="#"><img src="../assets/images/img_logo.png" alt=""></a></li>
      <li><a href="#"><img src="../assets/images/img_logo.png" alt=""></a></li>
      <li><a href="#"><img src="../assets/images/img_logo.png" alt=""></a></li>
    </ul>
  </section>
</template>

<script>
export default {
  name: 'CompanyBlock',
};
</script>

<style lang="scss" scoped>
  @import "../assets/stylesheets/_mixin";

  section {
    @include container;
    padding: {
      top: 60px;
      bottom: 60px;
    }
  }

  h2 {
    @include title;
  }
  ul {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    margin-top: 30px;
    padding: 0;
  }

  li {
    margin: 15px;
  }
</style>
