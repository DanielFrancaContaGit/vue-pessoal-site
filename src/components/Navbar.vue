<script setup>
  import { ref } from 'vue';
  const isDrowOpen = ref(false)

</script>

<template>
  <v-navigation-drawer v-model="isDrowOpen">
    <v-list>

    <v-list-subheader @click="isDrowOpen = !isDrowOpen">Menu</v-list-subheader>

    <v-list-item href="#home" @click="isDrowOpen = !isDrowOpen" prepend-icon="mdi-home">Home</v-list-item>

    <v-list-item prepend-icon="mdi-account"
    href="#sobremim" @click="isDrowOpen = !isDrowOpen"
    >Sobre min</v-list-item>
     
    <v-list-item prepend-icon="mdi-file-document-multiple"
    href="#projetos" @click="isDrowOpen = !isDrowOpen"
    >Projetos</v-list-item>

    <v-list-item prepend-icon="mdi-email"
    href="#footer" @click="isDrowOpen = !isDrowOpen"
    >Contato</v-list-item>

    </v-list>
  </v-navigation-drawer>
  <v-app-bar flat :elevation="2">
    <v-app-bar-nav-icon @click="isDrowOpen = !isDrowOpen" ></v-app-bar-nav-icon>
    <v-app-bar-title>
      <v-card href="#home">
        Home
      </v-card>  
    </v-app-bar-title>
    <div class="d-none d-md-block">
     
    <v-btn href="#sobremim">
      Sobre mim
    </v-btn>
    
    <v-btn href="#projetos">
      Projetos
    </v-btn>
     
    <v-btn class="mr-5" href="#footer">
      contato
    </v-btn>

    </div>
    <div class="ml-20"/>
  </v-app-bar>
</template>