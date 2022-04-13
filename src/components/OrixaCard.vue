<script setup>
import OrixaAvatar from './OrixaAvatar.vue'
import OrixaInfo from './OrixaInfo.vue'
</script>

<script>
export default {
  props: ['orixa']
}
</script>

<template>
  <div class="card">
    <OrixaAvatar :image="orixa.image" />
    <OrixaInfo :orixa="orixa" />
  </div>
</template>

<style scoped>
.card {
  background-color: #fff;
  border-radius: 20px;
  box-shadow: rgb(100 100 111 / 20%) 0px 7px 29px 0px;
  overflow: hidden;
  height: 770px;
  max-height: 770px;
  min-width: 400px;
}
</style>
