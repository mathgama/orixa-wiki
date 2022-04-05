<script setup>
import OrixaWiki from './components/OrixaWiki.vue'
</script>

<template>
  <main>
    <OrixaWiki />
  </main>
</template>

<style>
@import './assets/base.css';

#app {
  max-width: 800px;
  margin: 0 auto;
  padding: 2rem;

  font-weight: normal;
}

body {
  background-color: #dadfe8;
  display: flex;
  place-items: center;
}
</style>
