<template>
  <div class="error d-flex align-center justify-center" style="height: 100vh">
    <v-card class="ma-auto w-50 text-center pa-8">
      <v-card-title>
        Error: {{ error.statusCode }}
      </v-card-title>
      <v-card-title>
        {{ error.statusMessage }}
      </v-card-title>
      <v-btn @click="clearErr">
        back to homepage
      </v-btn>
    </v-card>

  </div>
</template>

<script lang="ts" setup>

defineProps(["error"])

const clearErr = () => {
  clearError({redirect: "/"})
}
</script>


<style scoped>


</style>