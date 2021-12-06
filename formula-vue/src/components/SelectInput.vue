<template>

  <div class="hello">

  <label>{{ msg }}</label>

    <select v-model="select">

  <option disabled value="">Veuillez séléctionnez une option</option>

  <option>Etudiant</option>

  <option>Salarié</option>

</select>

<MenuSelect />
<DateInput />
<CheckBoxInput />

  </div>

</template>

<script>

import MenuSelect from "./MenuSelect.vue";
import CheckBoxInput from "./CheckBoxInput.vue";
import DateInput from "./DateInput.vue";

export default {

  name: "SelectInput",
  
  components: {
      MenuSelect,
      CheckBoxInput,
      DateInput

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
