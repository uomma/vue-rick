<script >
import axios from 'axios';
import { store } from './store'
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter
  },
  data() {
    return {
      store
    }


  },
  methods: {

    search(){
      axios.get('https://rickandmortyapi.com/api/character', {
        params:{
          name: store.searchKey,
          status: store.searchStatus,
        }
      })
      .then((response) => {
        console.log(response);
        this.store.characters = response.data.results;
        this.store.charactersFound = response.data.results.length;
      })
    }
  },

  created() {
    this.search()
   
  },
}
</script>

<template>
  <AppHeader />
  <AppMain @algo="search" />
  <AppFooter />
</template>

<style lang="scss"></style>
