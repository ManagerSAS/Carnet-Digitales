<template>
    <v-container fluid class="mt-15">
        <v-row justify="center" align="center">
            <v-col cols="12" sm="12" md="10" lg="10" justify="center" align="center">
                <h1 class="titles">Inventario Tarjetas/Carnet Digitales</h1>
            </v-col>
        </v-row>
        <v-row justify="center" align="center">
            <v-col cols="12" sm="10" md="10" lg="5">
                <v-text-field
                    label="Append outer"
                    outlined
                    dense
                    rounded
                    hide-details
                    prepend-inner-icon="mdi-magnify"
                ></v-text-field>
            </v-col>
        </v-row>
        <v-row justify="center" align="center">
            <v-col justify="center" align="center" cols="12" md="10" sm="12" lg="8">
                <v-row justify="center" align="center">
                    <v-col cols="12" sm="12" md="3" lg="3" v-for="({Cant, text}, index) in Inventario" :key="index">
                        <div justify="center" align="center">
                            <div class="circle Cant pa-10">
                                {{Cant}}
                            </div>
                            <div>
                                <p class="text">{{text}}</p>
                            </div>
                        </div>
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
        Inventario:[
          {Cant:'50', text:'name'},
          {Cant:'22', text:'Crear Plantilla'},
          {Cant:'33', text:'Crear Nueva Tarjeta', },
          {Cant:'2', text:'Generar Informe'},
          {Cant:'50', text:'name'},
          {Cant:'22', text:'Crear Plantilla'},
          {Cant:'33', text:'Crear Nueva Tarjeta', },
          {Cant:'2', text:'Generar Informe'},
        ]
       }
     }
   }
</script>