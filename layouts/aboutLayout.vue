<script lang="ts" setup>

</script>

<template>
  <div class="about_layout">
    <v-layout>
      <v-app-bar>
        <ul class="d-flex" style="gap: 30px">
          <nuxt-link :to="{name: 'index'}">Home</nuxt-link>
          <nuxt-link :to="{name: 'about'}
">About
          </nuxt-link>
          <nuxt-link :to="{name: 'profile'}">
            Profile
          </nuxt-link>
          <nuxt-link :to="{name: 'products'}"
          >Blogs
          </nuxt-link>
        </ul>
      </v-app-bar>
      <v-main>
        <slot></slot>
      </v-main>
      <v-footer :app="true">
        <ul class="d-flex" style="gap: 30px">
          <nuxt-link :to="{name: 'index'}">Home</nuxt-link>
          <nuxt-link :to="{name: 'about'}
">About
          </nuxt-link>
          <nuxt-link :to="{name: 'profile'}">
            Profile
          </nuxt-link>
          <nuxt-link :to="{name: 'products'}"
          >Blogs
          </nuxt-link>
        </ul>
      </v-footer>
    </v-layout>

  </div>
</template>

<style scoped>

</style>