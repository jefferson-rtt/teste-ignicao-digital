<template>
  <div class="container-main">
    <Menu class="menu"/>
    <Dashboard class="dashboard" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Menu from '@/components/Menu.vue'
import Dashboard from '@/components/Dashboard.vue'


export default defineComponent({
  name: "App",
  components: {Menu, Dashboard
  },
});
</script>

<style>
.container-main{
  max-width: 1600px;
  margin: 0 auto;
  display: grid;
  grid-auto-flow: column;
  grid-template-columns: auto 1fr;
  grid-gap: 20px;

  box-sizing: border-box;

  padding: 0 20px;
}

.dashboard{
  width: 100%;
  margin: 10px 0;
}

</style>
