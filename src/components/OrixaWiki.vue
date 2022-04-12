<script setup>
import OrixaCard from './OrixaCard.vue'
import OrixaList from './OrixaList.vue'

import orixasData from '../data.json'
</script>

<script>
export default {
  data() {
    return {
      selected: null
    }
  },

  created() {
    if (!this.selected) this.selected = orixasData[0]
  },

  methods: {
    selectOrixa(selectedId) {
      this.selected = orixasData.filter((el) => el.id == selectedId)[0]
    }
  }
}
</script>

<template>
  <div class="wiki">
    <OrixaCard :name="selected.name" :image="selected.image" />
    <OrixaList :selectedId="selected.id" @selectOrixa="selectOrixa" />
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
