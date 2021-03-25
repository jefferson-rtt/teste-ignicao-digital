<template>
  <div class="grid">
    <div class="container-dashboard">
        <Navbar class="navbar"/>
        <BreadCrumbs class="results"/>
    </div>
    <div class="frame">
      <Filters />
      <FrameGrid />
    </div>
    <Footer  class="footer"/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Navbar from '@/components/navegation/Navbar.vue'
import BreadCrumbs from '@/components/navegation/BreadCrumbs.vue'
import Filters from '@/components/dashboard/Filters.vue'
import FrameGrid from '@/components/dashboard/FrameGrid.vue'
import Footer from '@/components/dashboard/Footer.vue'

export default defineComponent({
  components: {
    Navbar, BreadCrumbs, Filters, FrameGrid, Footer
  }
})
</script>

<style scoped>
.grid{
  display: grid;
  grid-auto-flow: row;
  grid-template-rows: auto;
  grid-template-columns: 1fr;
  grid-gap: 20px;
  box-sizing: border-box;
}
.navbar{
  margin-bottom: 10px;
}

.frame{
  display: grid;
  grid-auto-flow: column;
  grid-template-columns: auto 1fr;
  gap: 20px;
}

.footer{
  justify-self: center;
  margin-top: 5rem;
}
</style>