<template>
    <div>
        <h1>Quotes list</h1>
        <!-- <span>{{ quotesAmout }} Quotes</span> -->
    <ul class="quotes">
        <li v-for="quote in quotes" :key="quote.qt">
            <h1>{{ quote.quote }}</h1>
            <h2>{{ quote.context }}</h2>
            <h3>{{ quote.theme }}</h3>
        </li>
    </ul>
    </div>
</template>

<script>
// import Vue from 'vue'
// import axios from 'axios'
// import VueAxios from  'vue-axios'

// Vue.use(VueAxios,axios)
import json from '../assets/quotes.json'
export default {
    name: "QuotesList",

    data: function() {


        return { 
            quotes: json.quotes,
             };
 
    },

}
</script>
