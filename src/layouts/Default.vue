<template>

<v-app>

  <v-app-bar
    
    dense
    app>

    <v-app-bar-title class='headline me-2' >{{ $static.metadata.siteName }}</v-app-bar-title>
 
    <v-spacer></v-spacer>

    <v-btn to="/"  outlined class='me-2'>
      Примеры работ
    </v-btn>
   
    <v-btn to="/project/"  outlined class='me-2'>
      Примеры проектов
    </v-btn>
   
    <v-btn to="/contacts/" outlined class='me-2'>
      Контакты
    </v-btn>
 

   
 <!--
    <header class="header">
      <strong>
        <g-link to="/">{{ $static.metadata.siteName }}</g-link>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/about/">About</g-link>
      </nav>
    </header>

 -->



  </v-app-bar>

  <!-- Sizes your content based upon application components -->
  <v-main>

    <!-- Provides the application the proper gutter -->
    <v-container fluid fill-height >

      <!-- If using vue-router -->
      <slot  />
    </v-container>
  </v-main>

   <v-footer padless app>
    <v-col
      class="text-center"
      cols="12"
    >
      {{ new Date().getFullYear() }} — <strong>{{ $static.metadata.siteName }}</strong>
    </v-col>
  </v-footer>
</v-app>




</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>

</style>
