<template>
  <Layout>
  <v-card
    class=" mx-auto"
    tile
  >


    <v-list>
      <v-list-item v-for="item in $page.files.edges"
      :key="item.node.id"
      :href="'http://localhost:1337' + item.node.file[0].url">
        <v-list-item-icon>
          <v-icon >
            mdi-file
          </v-icon>
        </v-list-item-icon>
        <v-list-item-content>
          <v-list-item-title>{{ item.node.Description}}</v-list-item-title>
        </v-list-item-content>
      </v-list-item>



    </v-list>
  </v-card>
  </Layout>
</template>

<page-query>
query 
{
  files: allStrapiProjects
  {
    edges
    {
      node
      {
        id
        Description
        file
        {
          url
        }
      }
    }
  }
}

</page-query>



<script>
export default {
  metaInfo: {
    title: 'Примеры работ'
  }
}
</script>
