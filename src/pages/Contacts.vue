<template>
  <Layout>
   <v-card
    class=" mx-auto"
    max-width="300"
    
    tile
    
  >


    <v-list>
      <v-list-item>
        <v-list-item-icon>
          <v-icon >
            mdi-phone
          </v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title>(888) 8888888</v-list-item-title>

        </v-list-item-content>


      </v-list-item>

      <v-list-item>
        <v-list-item-action></v-list-item-action>

        <v-list-item-content>
          <v-list-item-title>(888) 88888888</v-list-item-title>

        </v-list-item-content>


      </v-list-item>

      <v-divider inset></v-divider>

      <v-list-item>
        <v-list-item-icon>
          <v-icon >
            mdi-email
          </v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title>@example.com</v-list-item-title>

        </v-list-item-content>
      </v-list-item>

      <v-list-item>
        <v-list-item-action></v-list-item-action>

        <v-list-item-content>
          <v-list-item-title>@example.com</v-list-item-title>
  
        </v-list-item-content>
      </v-list-item>

      <v-divider inset></v-divider>

      <v-list-item>
        <v-list-item-icon>
          <v-icon >
            mdi-map-marker
          </v-icon>
        </v-list-item-icon>

        <v-list-item-content>
          <v-list-item-title>Адресс</v-list-item-title>

        </v-list-item-content>
      </v-list-item>
    </v-list>
  </v-card>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Контакты'
  }
}
</script>