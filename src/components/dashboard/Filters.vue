<template>
  <div class="container-filters">
    <p>Filtros</p>
    <div class="menu">
      <div class="filtros">
        <form action="">
          <div class="prices">
            <p>Preços</p>
            <label>
              <input type="radio" name="Value">
              R$ 10.00
            </label>
            <label>
              <input type="radio" name="Value">
              R$ 10.00 - R$ 100.00
            </label>
            <label>
              <input type="radio" name="Value">
              R$ 100.00 - R$ 500.00
            </label>
            <label>
              <input type="radio" name="Value">
              R$ 500.00
            </label>
            <label>
              <input type="radio" name="Value" checked>
              Todos
            </label>
          </div>
          <div class="price-range">
            <label>
              <span>Valores R$ 1.99 - R$ 4.098</span>
              <input type="range" name="">
            </label>
          </div>
          <div class="categorias">
            <p>Categorias</p>
            <label class="results">
              <input type="checkbox" name=""> 
              Érico Rocha
              <span>1920</span>
            </label>
            <label class="results">
              <input type="checkbox" name=""> 
              Érico Rocha
              <span>1920</span>
            </label>
            <label class="results">
              <input type="checkbox" name=""> 
              Érico Rocha
              <span>1920</span>
            </label>
            <label class="results">
              <input type="checkbox" name=""> 
              Érico Rocha
              <span>1920</span>
            </label>
            <label class="results">
              <input type="checkbox" name=""> 
              Érico Rocha
              <span>1920</span>
            </label>
          </div>
          <div class="avaliacoes">
            <p>Avaliação</p>
            <span>
              <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
            </span>
            <span>
              <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="far fa-star"></i>
            </span>
            <span>
              <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="far fa-star"></i><i class="far fa-star"></i>
            </span>
          </div>
          <button type="reset">Limpar Filtros</button>
        </form>
      </div>
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
.container-filters{
  height: auto;
  width: 100%;
}

.menu{
  height: auto;
  padding: 0 20px;
  background: #FFFFFF;
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;

}

.prices{
  display: grid;
  grid-auto-flow: row;
  grid-gap: 15px;
  border-bottom: 1px solid #D6D6D6;
  padding-bottom: 15px;
}

.prices p{
  font-weight: 600;
  font-size: 1.125em;
  line-height: 1.3em;
}

.price-range{
  padding: 15px 0;
  border-bottom: 1px solid #D6D6D6;;
}

.price-range label{
  font-weight: 600;
  font-size: 1.125em;
  line-height: 1.3em;

  display: grid;
  grid-gap: 15px;
}

.categorias{
  padding: 15px 0;
  display: grid;
  grid-auto-flow: row;
  grid-gap: 10px;

  border-bottom: 1px solid #D6D6D6;

}
.categorias p{
  font-weight: 600;
  font-size: 1.125em;
  line-height: 1.3em;
}

.results{
  display: grid;
  grid-auto-flow: column;
  grid-template-columns: auto 1fr auto;
  grid-gap: 10px;
}

.avaliacoes{
  padding: 15px 0;
  display: grid;
  grid-auto-flow: row;
  gap: 10px;
}
.avaliacoes p{
  font-weight: 600;
  font-size: 1.125em;
  line-height: 1.3em;
}

.filtros form{
  display: flex;
  flex-direction: column;
}

.filtros form button{
  padding: 1rem;
  border: none;
  background: #696969;
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;
  color: #fff;
  outline: none;
  text-transform: uppercase;
  cursor: pointer;

  margin: 10px 0;

  justify-self: center;
}

.filtros form button:hover{
  lighting-color: chocolate;
}

</style>