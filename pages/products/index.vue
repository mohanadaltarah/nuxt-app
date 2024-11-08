<template>
  <div class="blogs">
    <h1>This is the products page</h1>
    <v-container v-if="data">
      <v-row>
        <v-col v-for="item in data.products" :key="item.id" cols="4">
          <v-card :to="{name: 'products-id', params: {id: item.id}}">
            <img :src="item.thumbnail" alt="" height="200" width="200">
            <v-card-title>
              {{ item.title }}
            </v-card-title>
            <v-card-text>
              {{ item.description }}
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script setup>

const {data} = useFetch('https://dummyjson.com/products')
</script>
