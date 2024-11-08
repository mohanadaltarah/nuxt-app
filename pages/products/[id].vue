<template>
  <div class="product-details">
    <v-card v-if="data">
      <img :src="data.thumbnail" alt="">
      <v-card-title>
        {{ data.title }}
      </v-card-title>
      <v-card-text>
        {{ data.description }}
      </v-card-text>
    </v-card>
  </div>
</template>

<script setup>
const {data, error} = useFetch(`https://dummyjson.com/products/${useRoute().params.id}`)
console.log(error)

if (error.value) {
  throw createError({statusCode: 404, statusMessage: "Product not Found", fatal: true})
}
</script>

<style scoped>

</style>