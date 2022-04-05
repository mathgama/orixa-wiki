<template>
  <nav class="list">
    <ul>
      <li class="active">
        <img src="../assets/img/obaluae_icon.png" alt="Obaluaê" />
        <span>Obaluaê</span>
      </li>
      <li>
        <img src="../assets/img/obaluae_icon.png" alt="Obaluaê" />
        <span>Obaluaê</span>
      </li>
      <li>
        <img src="../assets/img/obaluae_icon.png" alt="Obaluaê" />
        <span>Obaluaê</span>
      </li>
      <li>
        <img src="../assets/img/obaluae_icon.png" alt="Obaluaê" />
        <span>Obaluaê</span>
      </li>
    </ul>
  </nav>
</template>

<style scoped>
.list {
  max-width: 240px;
}

.list ul {
  padding: 0;
  list-style-type: none;
}

.list li {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 10px;
  background-color: #6b727a;
  color: #fff;
  cursor: pointer;
  border-top-left-radius: 30px;
  border-bottom-left-radius: 30px;
  box-shadow: rgb(100 100 111 / 20%) 0px 7px 29px 0px;
  min-width: 190px;
  min-height: 70px;
  margin-bottom: 10px;
  transition: 0.15s ease-in-out;
}

.list li:hover {
  transform: scale(1.05);
}

.list .active {
  background-color: #669afa;
}

.list span {
  padding-right: 20px;
}
</style>
