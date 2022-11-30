<template>
    <v-container fluid class="mt-15"> 
        <v-row justify="center" align="center">
            <v-col cols="12" sm="12" md="10" lg="10" justify="center" align="center">
                <h1 class="titles">Inventario Tarjetas/Carnet Digitales</h1>
            </v-col>
        </v-row>
        <v-row align="center" justify="center" class="mt-15">
            <v-col cols="12" sm="12" md="10" lg="8">
                <v-row align="center" justify="center">
                    <v-col cols="12" sm="12" md="6" lg="6">
                        <v-text-field
                            label="Nombre Empresa"
                            placeholder="Nombre Empresa"
                            outlined
                            rounded
                            hide-details
                            dense
                        ></v-text-field>
                    </v-col>
                    <v-col cols="12" sm="12" md="6" lg="6">
                        <v-text-field
                            label="Cantidad"
                            placeholder="Cantidad"
                            outlined
                            rounded
                            hide-details
                            dense
                        ></v-text-field>
                    </v-col>
                    <v-col cols="12" sm="12" md="6" lg="6">
                        <v-file-input
                            label="Outlined"
                            placeholder="Placeholder"
                            outlined
                            rounded
                            dense
                            hide-details
                        ></v-file-input>
                    </v-col>
                    <v-col cols="12" sm="12" md="6" lg="6">
                        <v-select
                            label="Platilla"
                            placeholder="Placeholder"
                            :items="items"
                            outlined
                            rounded
                            dense
                            hide-details
                        ></v-select>
                    </v-col>
                </v-row>
            </v-col>
        </v-row>
        <v-row justify="center" align="center">
            <v-col justify="center" align="center" cols="12" sm="12" md="3" lg="3"> 
                <div>
                    <h2 class="sub-titles mb-5 mt-5">Previsualización Platilla</h2>
                </div>
                <iframe height="600" width="100%" src="https://mitarjetadigital.co/Manager/Abel_Rodriguez_Gerente/" frameborder="0"></iframe>
                <!-- <img src="..s/../static/TarjetaDigital.png" alt="" srcset=""> -->
            </v-col>    
        </v-row>
        <v-row justify="center" align="center">
            <v-col justify="center" align="center" cols="12" sm="12" md="3" lg="3">
                <v-btn color="blue lighten-1 white--text">
                    Crear Tarjeta
                </v-btn>
            </v-col>
        </v-row>
    </v-container>
</template>
<script>
  export default {
    data: () => ({
      items: ['Foo', 'Bar', 'Fizz', 'Buzz'],
    }),
  }
</script>