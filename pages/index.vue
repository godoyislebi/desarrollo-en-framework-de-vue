<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <v-card class="logo py-4 d-flex justify-center">
        <NuxtLogo />
        <VuetifyLogo />
      </v-card>
      <v-card>
        <v-card-title class="headline">
          Desafío Desarrollo en framework de VUE
        </v-card-title>
        <v-card-text>
          <p>Requisitos:</p>
          <ul>
            <li>Debes utilizar un framework de UI.</li>
            <li>
              La aplicación DEBE ser renderizada por el servidor (SSR), por lo
              que se debe utilizar Nuxt.js
            </li>
            <li>
              El layout desarrollado queda a libertad de usted, sin embargo,
              deben existir al menos 1 vista:
              <ul>
                <li>
                  Vista con las tarjetas de los personajes, con los detalles más
                  importantes de estos.
                </li>
              </ul>
            </li>
            <li>La navegación debe ser mediante VueRouter (integrado en Nuxt.js).</li>
          </ul>
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn color="primary" nuxt to="/rickandmorty">
            Ver resultado del desafío realizado
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
