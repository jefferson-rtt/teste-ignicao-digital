<template>
  <div class="container">
    <Menu class="menu"/>
    <div class="dashboard">
      <Navbar class="navbar"/>
      <BreadCrumbs class="results"/>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Menu from '@/components/Menu.vue'
import Navbar from '@/components/dashboard/Navbar.vue'
import BreadCrumbs from '@/components/dashboard/BreadCrumbs.vue'

export default defineComponent({
  name: "App",
  components: {Menu, Navbar, BreadCrumbs
  },
});
</script>

<style>
.container{
  width: 1440px;
  margin: 0 auto;
  display: flex;
}
.menu{
  max-width: 280px;
}

.dashboard{
  width: 100%;
  margin: 20px;
}

</style>
