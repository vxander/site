<template>
  <Layout>
    
  
  <v-carousel hide-delimiters  height="100%" >
   
    <v-carousel-item 
      v-for="item in $page.imgs.edges"
      :key="item.node.id"
      

    >
      <v-img contain aspect-ratio="1.7"
  :lazy-src="'http://localhost:1337' + item.node.Img[0].url"

  :src="'http://localhost:1337' + item.node.Img[0].url"
></v-img>
    </v-carousel-item> 
    </v-carousel>
 <!--    <v-carousel-item 
      v-for="(color, i) in colors"
      :key="color"
    >
      <v-sheet
        :color="color"
        height="100%"
        tile
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
          <div class="text-h2">
            Slide {{ i + 1 }}
          </div>
        </v-row>
      </v-sheet>
    </v-carousel-item>






  </v-carousel>
-->
  </Layout>
</template>

<page-query>
query 
{
  imgs: allStrapiImages
  {
    edges
    {
      node
      {
        id
        Img
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

<style>

</style>
