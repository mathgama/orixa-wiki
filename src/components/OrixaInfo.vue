<script>
export default {
  props: ['name']
}
</script>

<template>
  <div class="name">
    <h1>{{ this.name }}</h1>
  </div>
  <div class="attributes">
    <p>Senhor da cura, da evolução e da passagem.</p>
    <ul>
      <li><b>Saudação</b> – Atotô</li>
      <li><b>Sincretismo</b> – São Roque e São Lázaro</li>
      <li><b>Símbolos</b> – Xaxará e filá</li>
      <li><b>Elemento</b> – Terra</li>
    </ul>
  </div>
</template>

<style scoped>
.name {
  top: -20px;
  padding: 10px 30px;
  background-color: #fff;
  border-radius: 20px 20px 0px 0px;
}

.name h1 {
  font-size: 1.5em;
  font-weight: bold;
  color: #000;
  border-bottom: 1px solid #000;
}

.attributes {
  top: -20px;
  width: 400px;
  padding: 0px 30px;
}

.attributes ul {
  margin-top: 10px;
  list-style-type: none;
  padding: 0px;
}

.attributes li > b {
  font-weight: bold;
}
</style>
