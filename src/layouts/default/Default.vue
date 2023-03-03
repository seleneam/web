<template>
  <v-app>
    <default-bar />
    <menuvue />
    <default-view />
  </v-app>
</template>

<script setup>
  import DefaultBar from './AppBar.vue'
  import DefaultView from './View.vue'
  import menuvue from './Menu.vue';
</script>
