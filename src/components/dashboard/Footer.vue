<template>
  <div class="container-footer">
    <div class="box">
      <a href="#"><i class="fas fa-chevron-left"></i></a>
      <ul class="pages">
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li class="active">4</li>
        <li>5</li>
        <li>6</li>
        <li>7</li>
        <li>8</li>
      </ul>
      <a href="#"><i class="fas fa-chevron-right"></i></a>
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
.conainer-footer{
  width: 100%;
  height: 100%;
}

ul{
  padding: 0;
}

.box{
  height: auto;
  display: grid;
  grid-auto-flow: column;
  grid-gap: 10px;
}

.pages{
  display: grid;
  grid-auto-flow: column;
  /* grid-gap: 10px; */
  background: #EDEDED;
  border-radius: 50px;
}

.pages li{
  display: list-item;
  font-size: 1.125em;
  padding: .8rem 1.2rem;
  transition: all .2s;
  cursor: pointer;
}
.pages .active{
  display: block;
  background: #686868;
  font-size: 1.125em;
  border-radius: 50%;
  color: #fff;
}
.pages li:hover{
  background: #686868;
  border-radius: 50%;
  color: #fff;

}

.box > a{
  background: #EDEDED;
  align-self: center;

  padding: 1rem 1.2rem;
  border-radius: 50%;
}
</style>