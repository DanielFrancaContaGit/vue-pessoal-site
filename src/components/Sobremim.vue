<template>
    <v-container flat id="sobremim">
        <v-row align="center" justify="center" class="ma-0">
            <h1 class="text-h2 mb-10 text-blue-grey-darken-4">-------</h1>
        </v-row>
        <v-card 
        variant="outlined"
        class="h-auto rounded"
        color="blue-grey-darken-4"
        >
        <div class="d-flex flex-column flex-sm-row h-100 justify-center">
            <v-avatar
                color="grey"
                size="330"
                class="ma-3 my-5 d-none d-md-block rounded"
                >     
                <v-img src="https://avatars.githubusercontent.com/u/57536006?v=4" />
            </v-avatar>
            <div class="d-flex flex-column pr-md-20 pl-md-5">
                <v-card-title class="text-h6 mt-5 font-weight-light">
                    O que eu sou?
                </v-card-title>
                <v-card-title class="text-h5 font-weight-regular  text-wrap">
                    Eu sou Daniel Franca, um estudante de engenharia e desenvolvedor web.
                </v-card-title>
                <v-card-text>
                    Oi, sou um estudante de Engenharia Eletrônica e apaixonado por desenvolvimento.
                    Aqui, compartilho meu percurso de aprendizado, explorando as interseções entre eletrônica
                    e programação. De projetos simples a desafios mais complexos, cada linha de código representa
                    meu compromisso com o crescimento profissional. Meu interesse abrange áreas como backend, frontend,
                    devops e machinelearning. Estou sempre em busca de novas ferramentas e linguagens para expandir
                    minhas habilidades. 
                </v-card-text>
                <v-card-actions class="">
                    <v-btn href="https://github.com/DanielFrancaContaGit" target="_blank">
                        github
                    </v-btn>
                
                    <v-btn href="https://www.linkedin.com/in/daniel-silva-franca" target="_blank">
                        linkedin
                    </v-btn>
                </v-card-actions>
            </div>
        </div>
        </v-card>
    </v-container>
</template>