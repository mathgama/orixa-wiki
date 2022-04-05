<script setup>
import OrixaCard from './OrixaCard.vue'
import OrixaList from './OrixaList.vue'
</script>

<template>
  <div class="wiki">
    <OrixaCard />
    <OrixaList />
  </div>
</template>

<style scoped>
.wiki {
  display: flex;
  gap: 30px;
}

@media (max-width: 768px) {
  .wiki {
    flex-direction: column;
  }
}
</style>
