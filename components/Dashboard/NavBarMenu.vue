<template>
  <div>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      fixed
      app
      dark
    >
        <template >
          <div justify="center" align="center" class="ma-5 mt-10 logo">
            <img src="../../static/Logo-Manager.png" alt="" srcset="" >
          </div>
        </template>
        <v-list
        dense
        nav
      >
        <v-list-item
          v-for="item in items"
          :key="item.title"
          link
          :to="item.to"
        >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title >{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar app flat dark >
        <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
        <v-toolbar-title>Tarjetas Digitales</v-toolbar-title>
        <v-spacer></v-spacer>
        <div>
          <v-btn icon class="rounded-xl" >
            <img src="../../static/Logo-Manager.png" width="30" alt="" srcset="" >
          </v-btn>
        </div>
    </v-app-bar>
  </div>
</template>
  
  <script>
  export default {
    data () {
      return {
        drawer: true,
        items: [
          {
            icon: 'mdi-home-outline',
            title: 'Dashboard',
            to: '/Dashboard/Panel'
          },
          {
            icon: 'mdi-web-plus',
            title: 'Crear Plantilla',
            to: '/Dashboard/CreateTheme'
          },
          {
            icon: 'mdi-database-outline',
            title: 'Inventario',
            to: '/Dashboard/Inventario'
          },
          {
            icon: 'mdi-book-plus-multiple-outline',
            title: 'Crear Nueva Tarjeta',
            to: '/Dashboard/CreateCard'
          },
          {
            icon: 'mdi-book-edit-outline',
            title: 'Generar Informe',
            to: '/Dashboard/GenerateReport'
          }
        ],
      }
    }
  }
  </script>
  