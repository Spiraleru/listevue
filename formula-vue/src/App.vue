<template>
<h1 :style="{color:colorie}">Coucou</h1>
  <div id="app">

    <img alt="Vue logo" src="./assets/logo.png" />
    <Bouttons msg="" v-on:validation="step='step 2'"/>
    <div v-if="step === 'step 1'">

<h1>Inscription</h1>
    <TextAreaInput msg="description " />
    <button v-on:click="step='step 2'">Valider</button>
</div>

<div v-if="step === 'step 2'">

<h1>Information</h1>
    <SelectInput msg="profession " />
<button v-on:click="step='step 3'">Valider</button>
</div>

<div v-if="step === 'step 3'">
<h1>Paiement</h1>
   
  
<button v-on:click="step='step 1'">Valider</button>
</div>
  </div>
<h1 :style="{color:color}">Change la couleurs</h1>
<Couleur msg='bleu' v-on:click="color='noir'"/>
<Couleur msg='noir' v-on:click="color='yellow'"/>
<Couleur msg='jaune' v-on:click="color='bleu'"/>
</template>

<script>


import TextAreaInput from "./components/TextAreaInput.vue";

import SelectInput from "./components/SelectInput.vue";

import Bouttons from "./components/Bouttons.vue";

import Couleur from "./components/Couleur.vue";
export default {

 

  name: "App",

  components: {

    Couleur,
    TextAreaInput,
    SelectInput,
    Bouttons,

  },

  data: function () {

    return {
      color:'',
colorie:'red',
step:'step 1',
  
      name: "HUHO",

      email: {

        value: "huho@gmail.com",

      },

    };

  },

};

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
