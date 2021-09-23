<template>
  <div id="app">
  <QuotesList />
  </div>
</template>

<script>
import QuotesList from './components/QuotesList'
export default {
  name: "App", 
  components: {
    QuotesList
  },

};
</script>

<style>
#app {
  font-family: Arial, Helvetica, sans-serif;
  text-align: center;
  color: black;
  margin-top: 60px;
}
</style>