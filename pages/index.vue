<template>
  <div class="home">
    <h1>Home Page</h1>
    <img alt="" src="/images/profil-min.png">
    <v-btn>Test</v-btn>
  </div>

</template>

<script setup>
useHead({
  title: "Home Page",
  meta: [{
    name: "description",
    content: "A home for aspiring young people",
  }, {
    name: "keywords",
    content: "self-development, strong, confident, hard-worker"
  }]
})


</script>


<style scoped>
img {
  width: 300px;
}
</style>