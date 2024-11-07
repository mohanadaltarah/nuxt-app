<template>
  <div class="nav">
    <nav style="width: 100%; height: 70px; background-color: aquamarine">
      <nuxt-link :to="{name: 'index'}">Home</nuxt-link>
      <nuxt-link :to="{name: 'about'}
">About
      </nuxt-link>
      <nuxt-link :to="{name: 'profile'}">
        Profile
      </nuxt-link>
      <nuxt-link :to="{name: 'blogs'}"
      >Blogs
      </nuxt-link>
    </nav>

  </div>
</template>

<script setup>

import {onMounted} from "vue";
import {useRouter} from "vue-router";

const router = useRouter();

onMounted(() => {
  console.log(router.options.routes)
})

</script>

<style scoped>

nav {
  padding: 20px;
  display: flex;
  gap: 1rem;
}

.router-link-active.router-link-exact-active {
  color: red;
}
</style>