<template>
  <div class="home">
    <h1>Home Page</h1>
    <img alt="" src="/images/profil-min.png">
    <v-btn>Test</v-btn>
  </div>

</template>

<script setup>

console.log(useCookie("user").value);

useCookie("user", {
  expires: new Date(Date.now() + 1000)
}).value = "test";


</script>


<style scoped>
img {
  width: 300px;
}
</style>