<script setup>
    const icons = [
      {
        icon: 'mdi-github',
        name: 'github',
        url: 'https://github.com/DanielFrancaContaGit'
      },
      {
        icon: 'mdi-linkedin',
        name: 'linkedin',
        url: 'https://www.linkedin.com/in/daniel-silva-franca'
      },
    ]
</script>

<template>
    <v-card id="home" class="h-screen">
        <v-img
            aspect-ratio="16/9"
            cover
            src="../assets/abstract-2d-colorful-wallpaper-with-grainy-gradients.jpg"
            >
            <v-container class="d-flex flex-column h-100  align-center justify-center">
                <v-card-title class="text-white text-md-h2 text-h4 text-wrap text-center">
                    Bem vindo ao meu site
                </v-card-title>
                <v-card-title class="text-white text-subtitle-1 mt-3 mb-20">
                    Feito por Daniel França
                </v-card-title>
                <v-alert-title>
                    <v-row class="my-6">
                        <v-card
                          v-for="{ icon, url, name } in icons"
                          :href="url"
                          target="_blank"
                          link
                          variant="text"
                          class="mx-4"
                        >
                            <v-btn
                            :prepend-icon="icon"
                            elevation="4"
                            variant="flat"
                            >
                        {{ name }}
                        </v-btn>
                        </v-card>
                    </v-row>
                </v-alert-title>
            </v-container>
        </v-img>
    </v-card>
</template>