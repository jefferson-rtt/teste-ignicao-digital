<template>
  <Menu/>
  <Navbar/>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import Menu from '@/components/Menu.vue'
import Navbar from '@/components/Navbar.vue'

export default defineComponent({
  name: "App",
  components: {Menu, Navbar
  },
});
</script>

<style>

</style>
