<template>
  <div id="app">
    <app-header/>
    <main>
      <app-grid/>
    </main>
    <footer>
      <app-footer/>
    </footer>
  </div>
</template>

<script>
 import appHeader from './components/appHeader.vue';
 import appGrid from './components/appGrid.vue'
 import AppFooter from './components/AppFooter.vue';

export default {
  name: 'App',
  components: {
    appHeader,
    appGrid,
    AppFooter,
  }
}
</script>

<style lang="scss">
@import './style/variables';
@import './style/general';

</style>
