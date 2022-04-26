<script>
import orixasData from "../data.json";

export default {
  props: ["selectedId"],

  data() {
    return {
      orixas: orixasData,
    };
  },
};
</script>

<template>
  <nav class="list">
    <ul>
      <li
        v-for="orixa in orixas"
        :key="orixa.id"
        :class="orixa.id == selectedId ? 'active' : ''"
        @click="$emit('selectOrixa', orixa.id)"
      >
        <img :src="`/assets/img/${orixa.icon}`" :alt="orixa.name" />
        <span>{{ orixa.name }}</span>
      </li>
    </ul>
  </nav>
</template>

<style scoped>
.list {
  max-width: 400px;
}

.list ul {
  padding: 0;
  list-style-type: none;
  display: flex;
  gap: 15px;
  flex-wrap: wrap;
  min-width: 300px;
}

.list li {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 10px;
  background-color: #6b727a;
  color: #fff;
  cursor: pointer;
  box-shadow: rgb(100 100 111 / 20%) 0px 7px 29px 0px;
  min-height: 83px;
  transition: 0.15s ease-in-out;
  flex-grow: 1;

  border-top-left-radius: 10px;
  border-bottom-left-radius: 10px;
  border-top-right-radius: 10px;
  border-bottom-right-radius: 10px;
  margin-bottom: 0px;
  width: 45%;
}

.list li:hover {
  transform: scale(1.05);
}

.list .active {
  background-color: #669afa;
}

.list span {
  padding-right: 10px;
  text-align: end;
  font-size: 15px;
}

@media (max-width: 768px) {
  .list ul {
    gap: 10px;
  }
}
</style>
