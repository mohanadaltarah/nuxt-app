<template>
  <div class="error d-flex align-center justify-center" style="height: 100vh">
    <v-card class="ma-auto w-50 text-center pa-8">
      <v-card-title>
        Error: {{ error.statusCode }}
      </v-card-title>
      <v-card-title>
        {{ error.statusMessage }}
        {{ error }}
      </v-card-title>
      <v-card-text>
        {{ error }}
      </v-card-text>
      <v-btn @click="$router.push({name: 'index'})">
        back to homepage
      </v-btn>
    </v-card>

  </div>
</template>

<script lang="ts" setup>

defineProps(["error"])
</script>


<style scoped>


</style>