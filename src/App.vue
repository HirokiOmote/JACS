<template>
  <div id="app">
    <header-block></header-block>
    <div>
      <build-block></build-block>
      <activity-block></activity-block>
      <example-block></example-block>
      <works-block></works-block>
      <invite-block></invite-block>
      <company-block></company-block>
      <footer-block></footer-block>
    </div>
  </div>
</template>

<script>
import HeaderBlock from './components/HeaderBlock';
import BuildBlock from './components/BuildBlock';
import ActivityBlock from './components/ActivityBlock';
import ExampleBlock from './components/ExampleBlock';
import WorksBlock from './components/WorksBlock';
import InviteBlock from './components/InviteBlock';
import CompanyBlock from './components/CompanyBlock';
import FooterBlock from './components/FooterBlock';

export default {
  name: 'app',
  components: {
    HeaderBlock,
    BuildBlock,
    ActivityBlock,
    ExampleBlock,
    WorksBlock,
    InviteBlock,
    CompanyBlock,
    FooterBlock,
  },
};
</script>

<style src="normalize.css"></style>
<style src="./assets/stylesheets/style.scss" lang="scss"></style>
<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
