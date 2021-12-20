<template>
  <div id="app">
    <Header/>

    <main>
      <MainTop/>
      <MainBottom/>
    </main>

    <footer>
      <FooterMenu/>
      <FooterContact/>
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import MainTop from "./components/MainTop.vue";
import MainBottom from "./components/MainBottom.vue";
import FooterMenu from "./components/FooterMenu.vue";
import FooterContact from "./components/FooterContact.vue";

export default {
  name: 'App',
  components: {
    Header,
    MainTop,
    MainBottom,
    FooterMenu,
    FooterContact,
  }
}
</script>

<style lang="scss">
@import './style/general.scss';
@import './style/common.scss';
@import './style/variables.scss';
</style>
