<template>
  <v-container>
    <h1>Product Detail</h1>
    <v-img :src="image" height="200px" contain></v-img>
    <h1>{{ productid }}. {{ title }}</h1>
    <h2>{{ price }}  $</h2> 
      
    <h3>{{ description }}</h3> 
    {{ category }}
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      productid: this.$route.params.id,
      description: this.$route.params.description,
      image: this.$route.params.image,
      price: this.$route.params.price,
      title: this.$route.params.title,
      category: this.$route.params.category,
    };
  },
};
</script>

<style></style>