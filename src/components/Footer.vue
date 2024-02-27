<script setup>
    const icons = [
      {
        icon: 'mdi-github',
        url: 'https://github.com/DanielFrancaContaGit'
      },
      {
        icon: 'mdi-linkedin',
        url: 'https://www.linkedin.com/in/daniel-silva-franca'
      },
    ]
</script>

<template>
    <v-row align="center" justify="center" class="ma-0">
      <h1 class="text-h2 mb-10 text-blue-grey-darken-4">-------</h1>
    </v-row>
    <v-footer
      id="footer"
      class="bg-blue-darken-4 text-center d-flex flex-column"
    >
      <v-row class="my-1">
        <v-card
          v-for="{ icon, url } in icons"
          :href="url"
          target="_blank"
          link
          variant="text"
          class="mx-4"
        >
            <v-btn
            :icon="icon"
            variant="text"
            ></v-btn>
        </v-card>
      </v-row>
  
      <div class="pt-0">
        Feito por Daniel França 
      </div>
  
      <v-divider></v-divider>
  
      <div>
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
      </div>
    </v-footer>
  </template>
  