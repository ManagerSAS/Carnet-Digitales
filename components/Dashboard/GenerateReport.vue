<template>
    <v-container fluid class="mt-15">
        <v-row justify="center" align="center">
            <v-col cols="12" sm="12" md="10" lg="10" justify="center" align="center">
                <h1 class="titles">Generar Reportes</h1>
            </v-col>
        </v-row>
        <v-row align="center" justify="center" class="mt-15">
            <v-col cols="12" sm="12" md="10" lg="8">
                <v-row align="center" justify="center">
                    <v-col cols="12" sm="12" md="4" lg="4">
                        <v-text-field
                            label="Nombre Empresa"
                            placeholder="Nombre Empresa / Persona"
                            outlined
                            rounded
                            hide-details
                            dense
                        ></v-text-field>
                    </v-col>
                    <v-col cols="12" sm="12" md="4" lg="4">
                        <v-text-field
                            label="Nombre Empresa"
                            placeholder="Nombre Empresa / Persona"
                            outlined
                            type="date"
                            rounded
                            hide-details
                            dense
                        ></v-text-field>
                    </v-col>
                    <v-col cols="12" sm="12" md="4" lg="4">
                        <v-text-field
                            label="Nombre Empresa"
                            placeholder="Nombre Empresa / Persona"
                            outlined
                            type="date"
                            rounded
                            hide-details
                            dense
                        ></v-text-field>
                    </v-col>
                </v-row>
            </v-col>
        </v-row>
        <v-row justify="center" align="center">
            <v-col justify="center" align="center" cols="12" sm="12" md="3" lg="3">
                <v-btn color="blue lighten-1 white--text">
                    Consultar
                </v-btn>
            </v-col>
        </v-row>
        <v-row justify="center" align="center">
            <v-col justify="center" align="center" cols="12" sm="12" md="10" lg="8">
                <v-card justify="center" align="center">
                    <v-row>
                        <v-col cols="12" sm="6" md="6" lg="6" justify="center" align="center">
                            <div class="sub-titles-table">
                                Nombre
                            </div>
                        </v-col>
                        <v-col cols="12" sm="6" md="6" lg="6" justify="center" align="center">
                            <div class="sub-titles-table">
                                Cantidad
                            </div>
                        </v-col>
                    </v-row>
                    <v-divider></v-divider>
                    <v-row>
                        <v-col cols="12" sm="6" md="6" lg="6" justify="center" align="center">
                            <div class="datas-report">
                                Manager S.A.S
                            </div>
                        </v-col>
                        <v-col cols="12" sm="6" md="6" lg="6" justify="center" align="center">
                            <div class="datas-report">
                                1.000
                            </div>
                        </v-col>
                    </v-row>
                </v-card>
            </v-col>
        </v-row>
        <v-row justify="center" align="center">
            <v-col justify="center" align="center" cols="12" sm="12" md="3" lg="3">
                <v-btn color="blue lighten-1 white--text">
                    Descargar Documento <v-icon>mdi-file-excel-outline</v-icon>
                </v-btn>
            </v-col>
        </v-row>
    </v-container>
</template>