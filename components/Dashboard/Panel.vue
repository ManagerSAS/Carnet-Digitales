<template>
    <v-container fluid class="mt-10">
      <v-row align="center" justify="center">
        <v-col align="center" justify="center" cols="12" sm="12" md="11" lg="10">
          <h1 class="titles">Panel de Control</h1>
        </v-col>
      </v-row>
      <v-row class="ma-5" align="center" justify="center">
        <v-col cols="12" sm="12" md="10" lg="10" align="center" justify="center">
          <v-row align="center" justify="center">
            <v-col cols="12" sm="12" md="4" lg="4" align="center" justify="center" v-for="({icon, text, href}, index) in Dashboard" :key="index"> 
                <v-card :to="href" max-width="200" max-height="200" class="ma-5 pa-10">
                  <v-icon class="ma-2">{{icon}} mdi-48px</v-icon>
                  <p>{{text}}</p>
                </v-card>
              </v-col>
            </v-row>
        </v-col>
      </v-row>
    </v-container>
</template>
<script>
   export default {
     data () {
       return {
        Dashboard:[
          {icon:'mdi-database-outline', text:'Inventario', href:'/Dashboard/Inventario'},
          {icon:'mdi-book-plus-multiple-outline', text:'Crear Plantilla', href:'/Dashboard/CreateTheme'},
          {icon:'mdi-web-plus', text:'Crear Nueva Tarjeta', href:'/Dashboard/CreateCard'},
          {icon:'mdi-book-edit-outline', text:'Generar Informe', href:'/Dashboard/GenerateReport' },
        ]
       }
     }
   }
</script>