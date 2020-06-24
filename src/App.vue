<template>
  <div id="app">
    <h1>Liste des inscrits</h1>
    <inscrits :liste="personnes"></inscrits>
  </div>
</template>

<script>
import Inscrits from "./components/Inscrits"
export default {
  name: "App",
  components: {
    Inscrits
  },
  data: function () {
    return {
      personnes: [
        {prenom: "Jean", nom: "Bréhat", age: 20},
        {prenom: "Léa", nom: "Prijean", age: 25},
        {prenom: "Chris", nom: "Martin", age: 38},
        {prenom: "Pierre", nom: "Petit", age: 16},
      ]
    }
  }
}
</script>

<style lang="css" scoped>
</style>
