<template>

  <div class="hello">

  <label>{{ msg }}</label>

    <input type="textarea" required >
    <RadioInput msg=""/>
    <TextInput msg="Prénom " />
    <TextInput msg="Nom " />

  </div>


</template>

<script>

import RadioInput from "./RadioInput.vue";
import TextInput from "./TextInput.vue";

export default {

  name: "TextAreaInput",

    components: {
            RadioInput,
            TextInput,
    },
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
