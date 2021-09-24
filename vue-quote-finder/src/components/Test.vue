<template>
  <div>
    <h1>Quote Finder with Vue</h1>
    <table>
      <tr class="ban">
        <th>Quote</th>
        <th>Context</th>
        <th>Source</th>
        <th>Theme</th>
      </tr>
      <tr v-for="(artist, x) in artists" :key="x" class="colls">
      <th class="qt">"{{artist.quote}}"</th>
      <th>{{artist.context}}</th>
      <th>{{artist.source}}</th>
      <th>{{artist.theme}}</th>
      </tr>
    </table>

  </div>
</template>
<script>
export default {
  name: 'Test',
  props: ['artists'],
}
</script>



<style scoped>

tr{
    height: 40px;
    width: 100%;
    padding: 15px;
    border: 1px solid saddlebrown;
    display: flex;
    justify-content: center;
    align-items: center;
  }  
  tr.ban{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
  }
  tr.colls{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
  }
  th{
    height: 40px;
    width: 100%;
    padding: 15px;
    border: 1px solid saddlebrown;
    display: flex;
    justify-content: center;
    align-items: center;
  }  
  th.qt{
    font-family: 'Courier New', Courier, monospace;
    
  }
a {
  color: #42b983;
}
</style>
