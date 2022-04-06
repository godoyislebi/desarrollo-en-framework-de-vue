<template>
  <v-row>
    <v-col
      v-for="personaje in personajesRick"
      :key="personaje.id"
      cols="6"
      sm="12"
      md="6"
    >
      <v-card :loading="loading" class="mx-auto my-12" max-width="374">
        <template slot="progress">
          <v-progress-linear
            color="deep-purple"
            height="10"
            indeterminate
          ></v-progress-linear>
        </template>

        <v-img height="250" :src="personaje.imagen"></v-img>

        <v-card-title>{{personaje.nombre}}</v-card-title>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'IndexRickAndMorty',
  data() {
    return {
      personajesRick: [
        {
          id: 1,
          nombre: 'Morty',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg',
        },
        {
          id: 2,
          nombre: 'Rick',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg',
        },
        {
          id: 3,
          nombre: 'Summer',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg',
        },
        {
          id: 4,
          nombre: 'Beth',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg',
        },
        {
          id: 5,
          nombre: 'Jerry',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg',
        },
      ],
    }
  },
}
</script>

<style></style>
