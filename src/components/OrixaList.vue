<template>
  <nav class="list">
    <ul>
      <li>
        <img src="../assets/img/ewa_icon.png" alt="Ewá" />
        <span>Ewá</span>
      </li>
      <li>
        <img src="../assets/img/exu_icon.png" alt="Exu" />
        <span>Exu</span>
      </li>
      <li>
        <img src="../assets/img/iansa_icon.png" alt="Iansã" />
        <span>Iansã</span>
      </li>
      <li>
        <img src="../assets/img/ibeji_icon.png" alt="Ibeji" />
        <span>Ibeji</span>
      </li>
      <li>
        <img src="../assets/img/iemanja_icon.png" alt="Iemanjá" />
        <span>Iemanjá</span>
      </li>
      <li>
        <img src="../assets/img/logunede_icon.png" alt="Logunedé" />
        <span>Logunedé</span>
      </li>
      <li>
        <img src="../assets/img/nana_icon.png" alt="Nanã Buruquê" />
        <span>Nanã Buruquê</span>
      </li>
      <li>
        <img src="../assets/img/oba_icon.png" alt="Obá" />
        <span>Obá</span>
      </li>
      <li class="active">
        <img src="../assets/img/obaluae_icon.png" alt="Obaluaê" />
        <span>Obaluaê</span>
      </li>
      <li>
        <img src="../assets/img/ogum_icon.png" alt="Ogum" />
        <span>Ogum</span>
      </li>
      <li>
        <img src="../assets/img/ossaim_icon.png" alt="Ossaim" />
        <span>Ossaim</span>
      </li>
      <li>
        <img src="../assets/img/oxala_icon.png" alt="Oxalá" />
        <span>Oxalá</span>
      </li>
      <li>
        <img src="../assets/img/oxossi_icon.png" alt="Oxossi" />
        <span>Oxossi</span>
      </li>
      <li>
        <img src="../assets/img/oxum_icon.png" alt="Oxum" />
        <span>Oxum</span>
      </li>
      <li>
        <img src="../assets/img/oxumare_icon.png" alt="Oxumaré" />
        <span>Oxumaré</span>
      </li>
      <li>
        <img src="../assets/img/xango_icon.png" alt="Xango" />
        <span>Xango</span>
      </li>
    </ul>
  </nav>
</template>

<style scoped>
.list {
  max-width: 240px;
  max-height: 84vh;
  overflow-y: scroll;
}

.list ul {
  padding: 0;
  list-style-type: none;
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
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
  min-width: 150px;
  max-width: 200px;
  min-height: 70px;
  transition: 0.15s ease-in-out;
  flex-grow: 1;
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

@media (max-width: 768px) {
  .list {
    max-width: 400px;
  }

  .list li {
    border-top-left-radius: 10px;
    border-bottom-left-radius: 10px;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
    margin-bottom: 0px;
  }
}
</style>
