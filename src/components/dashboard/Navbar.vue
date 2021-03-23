<template>
  <div class="container">
    <div class="tasks">
      <a href="#">
        <img src="@/assets/images/check-square.svg" alt="Todo">
      </a>
      <a href="#">
        <img src="@/assets/images/message-square.svg" alt="Conversar">
      </a>
      <a href="#">
        <img src="@/assets/images/calendar.svg" alt="Calendário">
      </a>
      <a href="#">
        <img src="@/assets/images/star.svg" alt="Favorito">
      </a>      
    </div>
    <div class="user">
      <span><img src="@/assets/images/bell.svg" alt="Notificações"></span>
      <span><img src="@/assets/images/search.svg" alt="Pesquisar"></span>
      <div class="profile">
        <p class="username">Nome do Usuário</p>
        <p class="description-user">Cliente VIP</p>
      </div>
      <img class="profile-photo" src="https://avatars.githubusercontent.com/u/69088071?s=460&u=736399602e4fbad29e62e788c567e4d089ec36a4&v=4" alt="Foto de Perfil">
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  setup () {
    

    return {}
  }
})
</script>

<style scoped>
.container{
  width: 100%;
  height: 70px;
  background: #FFFFFF;
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: space-between;

  padding: 0 20px;
}

.tasks{
  display: flex;
}

.tasks a{
  padding: 0 5px;
  margin: 0 5px;
  display: flex;
  align-items: center;
}

.tasks a img{
  width: 20px;
  height: 20px;
}

.user{
  display: flex;
  align-items: center;
}

.user span{
  margin: 0 10px;
}
.profile{
  margin-left: 20px;
}

.profile p{
  color: #2C2C2C;
  margin: 0;
  text-align: end;
}

.username{
  font-size: .85rem;
  line-height: 1rem;
}
.description-user{
  font-size: .70rem;
  line-height: 1rem;
}

.profile-photo{
  width: 60px;
  height: auto;

  border-radius: 50%;
  margin-left: 10px;

  box-shadow: -1px 1px 6px rgba(0, 0, 0, 0.235413);
}

</style>