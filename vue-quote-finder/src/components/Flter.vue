<template>
<div id="flter">
    <div class="btn-group pull-left">
        <p>Filter by Movies or Games</p>
        <input type="text" v-model="filters.searchQuoteTheme" />
    </div>
    {{ filtered_themes }}
</div>
</template>

<script>
export default {
  name: "Flter",
  data() {
    return {
            filters:{
                searchQuoteTheme: ''
            },
        }
    },
    props: ['artists'],
    computed: {
        // returns list of quotes based of theme filter
        filtered_themes(){
            let vm = this;
            if(!vm.filters.searchQuoteTheme){
                return [];
            }
            return vm.sortedThemes.filter(artists => {
                return artists.theme.toLowerCase().indexOf(vm.filters.searchQuoteTheme.toLowerCase()) != -1
            })
        },
        sortedThemes: function() {

            function compare(a, b) {

                if (a.theme < b.theme)
                    return -1;
                if (a.theme > b.theme)
                    return 1;

                return 0;
            }

            var sortedArr = this.artists.sort(compare);

            return sortedArr;
            
        }
        
    }
};
</script>