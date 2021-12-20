<template>
  <div id="app">
    <Header />
    <main>
      <!-- da fare -->
    </main>
    <FooterUp />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import FooterUp from "./components/FooterUp.vue";

export default {
  name: "App",
  components: {
    Header,
    FooterUp
  },
};
</script>

<style lang="scss">
  @import './style/general.scss';
  @import './style/ColorApp.scss';
  @import './style/commun.scss';

  // Da fare
  main{
    width: 100%;
    height: 200px;
    background: black;
  }
</style>
