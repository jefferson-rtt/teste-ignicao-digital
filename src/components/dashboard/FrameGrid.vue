<template>
  <div class="container-dash">
    <p>200 resultados encontrados</p>
    <div class="menu">
      <span class="search">
        <input type="search" placeholder="Buscar">
        <img src="@/assets/images/search.svg" alt="">
      </span>
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
.container-dash{
  width: 100%;
}

.menu{

}

.search{
  width: 100%;
  position: relative;
  display: flex;
  align-items: center;
}
.search input{
  width: 100%;
  height: 60px;
  padding: 0 40px 0 20px ;

  border: none;

  background: #FFFFFF;
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;
}

.search img{
  position: absolute;
  right: 20px;
}

</style>