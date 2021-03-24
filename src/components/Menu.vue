<template>
  <div class="container flex">
    <div class="menu-logo">
      <img src="@/assets/images/Brand.svg" alt="">
    </div>
    <div class="menu-select">
      <ul>
        <li>
          <a class="selected-area" href="#"> <img src="@/assets/images/home.svg" alt=""> Área do Cliente <img src="@/assets/images/chevron-down.svg" alt=""> </a>
          <ul class="dropdown">
            <li><a href="#">Outras Opções</a></li>
            <li><a href="#">Outras Opções</a></li>
          </ul>
        </li>
      </ul>
    </div>
    <div class="apps">
      <h4 class="apps-title">Apps</h4>
      <a href="#"><img src="@/assets/images/mail.svg"> Email</a>
      <a href="#"><img src="@/assets/images/message-square.svg"> Conversar</a>
      <a href="#"><img src="@/assets/images/check-square.svg"> Todo</a>
      <a href="#"><img src="@/assets/images/calendar.svg"> Calendário</a>
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
  height: 100%;
  box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.170509);

  box-sizing: border-box;
}

.flex{
  display: flex;
  flex-direction: column;
}

.menu-logo{
  display: inline-block;
  padding: 29px 44px;
}

.menu-select{
  align-self: center;
  text-align: center;
  width: 80%;
  position: relative;
}

.menu-select ul{
  padding-left: 0;
}

.selected-area{
  font-size: .95rem;
  color: #2C2C2C;
  display: flex;
  align-items: center;
  justify-content: space-around;
  background: #ECECEC;
  border-radius: 4px;
  height: 40px;

  align-self: center;
  position: relative;
}

.menu-select ul li:hover .dropdown{
  display: block;
}

.dropdown{
  display: none;
  position: absolute;
  width: 100%;
}

.dropdown li > a{
  display: list-item;
  padding: .7rem 2rem;
  background: #ECECEC;
}
.dropdown li > a:hover{
  background: #f2f2f2;
}

.apps{
  margin: 80px 0 0 35px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.apps a{
  padding: 5px 0;
  margin: 5px 0;
  color: #2C2C2C;
  display: flex;
  align-items: center;
  font-size: .95rem;
}
.apps a:hover{
  color: #f57830;
}

.apps a img{
  margin-right: 5px;
}

.apps-title{
  color: #999999;
  text-transform: uppercase;
}

</style>