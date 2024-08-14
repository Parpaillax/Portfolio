<template>
  <v-layout>
    <AppHeader></AppHeader>
    <v-main>
      <AboutMe></AboutMe>
    </v-main>
  </v-layout>
</template>

<script setup lang="ts">
import AppHeader from "~/components/header.vue";
import AboutMe from "../components/cv/CompAboutMe.vue";
</script>
