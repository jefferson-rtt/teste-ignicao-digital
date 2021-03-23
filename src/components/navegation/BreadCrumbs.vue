<template>
  <div class="container flex">
    <p>Resultados</p>
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
  max-width: 100%;
  height: 60px;

  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;

  padding: 0 20px;
}

.flex{
  display: flex;
  align-items: center;
}

</style>