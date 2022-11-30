<template>
    <v-container fluid class="mt-15">
        <v-row justify="center" align="center">
            <v-col cols="12" sm="12" md="10" lg="10" justify="center" align="center">
                <h1 class="titles">Crear Plantilla</h1>
            </v-col>
        </v-row>
        <v-row align="center" justify="center" class="mt-15">
            <v-col cols="12" sm="12" md="10" lg="8">
                <v-row align="center" justify="center">
                    <v-col cols="12" sm="12" md="6" lg="6">
                        <v-text-field
                            label="Nombre Platilla"
                            placeholder="Nombre Platilla"
                            outlined
                            rounded
                            hide-details
                            dense
                        ></v-text-field>
                    </v-col>
                    <v-col cols="12" sm="12" md="6" lg="6">
                        <v-select
                            label="Tipo Platilla"
                            placeholder="Placeholder"
                            :items="items"
                            outlined
                            rounded
                            dense
                            hide-details
                        ></v-select>
                    </v-col>
                </v-row>
                <v-row>
                    <v-col cols="12" >
                        <v-textarea
                            label="Código Paltilla"
                            placeholder="Código Platilla"
                            outlined
                            rounded
                            hide-details
                            dense
                        ></v-textarea>
                    </v-col>
                </v-row>
                <v-row justify="center" align="center">
                    <v-col justify="center" align="center" cols="12" sm="12" md="3" lg="3">
                        <v-btn color="blue lighten-1 white--text">
                            Crear Platilla
                        </v-btn>
                    </v-col>
                </v-row>
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