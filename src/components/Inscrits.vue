<template>
  <table border>
    <tr>
      <th>Prénom</th>
      <th>Nom</th>
      <th>Age</th>
    </tr>
    <tr v-for="(personne, index) in liste" :key="index">
      <td>{{ personne.prenom }}</td>
      <td>{{ personne.nom }}</td>
      <td>{{ personne.age }}</td>
    </tr>
  </table>
</template>

<script>
export default {
  name: "Inscrits",
  props: ["liste"]
}
</script>

<style scoped>
  th{
    background: lightgrey;
    font-size: 140%;
  }
  td{
    width: 10rem;
    text-align: center;
  }
</style>
