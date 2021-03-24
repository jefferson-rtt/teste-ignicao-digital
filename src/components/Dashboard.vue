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
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Navbar from '@/components/navegation/Navbar.vue'
import BreadCrumbs from '@/components/navegation/BreadCrumbs.vue'
import Filters from '@/components/dashboard/Filters.vue'
import FrameGrid from '@/components/dashboard/FrameGrid.vue'

export default defineComponent({
  components: {
    Navbar, BreadCrumbs, Filters, FrameGrid,
  }
})
</script>

<style scoped>
.grid{
  display: grid;
  grid-auto-flow: row;
  grid-template-rows: auto;
  grid-template-columns: 1fr;
  gap: 20px;
}
.navbar{
  margin-bottom: 10px;
}

.frame{
  display: grid;
  grid-auto-flow: column;
  grid-template-columns: 350px 1fr;
  gap: 20px;
}
</style>