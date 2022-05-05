<template>
  <div id="app">
    <app-header :menu="links"/>
    <main>
      <app-grid/>
    </main>
    <footer>
      <app-footer :pasta="pastificio"/>
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
  },
  data(){
    return {
      links:[
        {
            testo:'Home',
            link:'',
            active:false,
        },
        {
            testo:'Prodotti',
            link:'',
            active:true,
        },
        {
            testo:'Chi siamo',
            link:'',
            active:false,
        },
        {
            testo:'Contatti',
            link:'',
            active:false,
        }
      ],
      pastificio:[
        {
            text:'Il Pastificio',
            url:'#'
        },
        {
            text:'Grano',
            url:'#'
        },
        {
            text:'Filiera',
            url:'#'
        },
        {
            text:'100 anni di pasta',
            url:'#'
        },
        {
            text:'Sartoria della pasta',
            url:'#'
        },
      ]
    }
  }
}
</script>

<style lang="scss">
@import './style/variables';
@import './style/general';

</style>
