<script>
export default {
  props: ['image']
}
</script>

<template>
  <div
    class="avatar"
    v-bind:style="{ backgroundImage: 'url(' + image + ')' }"
  ></div>
</template>

<style scoped>
.avatar {
  width: 400px;
  height: 565px;
  background-size: contain;
  padding: 30px 30px 0;
}
</style>
