<template>
  <div>
   <h3>{{ h3tag }}</h3>
   <h2>{{ firstname }}</h2>
   <br>
   <input />
   <button v:onclick="">Add Name</button>
   <span v-bind:title="message">
    Hover your mouse over me for a few seconds
    to see my dynamically bound title!
  </span>
  </div>
</template>

<script>
export default {
  name: 'Test',
  props: {
    h3tag: String,
    firstname: String,
  },
  data: {
    message: 'You loaded this page on ' + new Date().toLocaleString()
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  color: black;
}
h2 {
  color: black;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
