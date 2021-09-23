<template>
  <div id="app">
  <QuotesList />
  <pagination
      :totalPages="5"
      :perPage="15"
      :currentPage="currentPage"
      @pagechanged="onPageChange"
    />
  </div>
</template>

<script>

import QuotesList from './components/QuotesList'
import Pagination from './components/Pagination.vue'


export default {
  name: "App", 
  components: {
    QuotesList,
    Pagination
  },
  data () {
    return{
      currentPage: 1,
    };
  },
  methods: {
    onPageChange(page) {
      console.log(page)
      this.currentPage = page;
    }
  }

}
</script>

<style>
#app {
  font-family: Arial, Helvetica, sans-serif;
  text-align: center;
  color: black;
  margin-top: 60px;
}
</style>