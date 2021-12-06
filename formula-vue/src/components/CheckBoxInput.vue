<template>
  <div class="hello">
    <label>{{ msg }}</label><br/>

      <input class="checkbox" type="checkbox" name="checkbox" value="market">  
      <label for="market">Marketing</label><br />

      <input class="checkbox" type="checkbox" name="checkbox" value="coding">  
      <label for="coding">Développement</label><br/>

      <input class="checkbox" type="checkbox" name="checkbox" value="design">  
      <label for="design">Webdesign</label><br/>

      <input class="checkbox" type="checkbox" name="checkbox" value="product">  
      <label for="product">Product Management</label>
    </div>
</template>

<script>

export default {

  name: "CheckBoxInput",

  props: {

    msg: String,

  },

};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
