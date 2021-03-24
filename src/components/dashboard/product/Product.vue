<template>
  <div class="box-product">
    <img class="image-product" src="@/assets/images/product-img.svg">
    <div class="content">
      <p class="header">FÓRMULA DE LANÇAMENTO</p>
      <p class="author">Por <strong>Érico Rocha</strong></p>
      <p class="description">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make
a type specimen book.</p>
    </div>
    <div class="price">
      <span class="classifications">
        3.4
        <img src="@/assets/images/Path.svg">
      </span>
      <p>R$2.500,00</p>
      <a class="heart btn" href="#">
        <img src="@/assets/images/heart.svg">
        <span>Amei</span>
      </a>
      <a class="buy btn" href="#">
        <img src="@/assets/images/shopping-bag.svg">
        <span>Comprar</span>
      </a>
    </div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>
.box-product{
  box-sizing: border-box;

  width: 100%;

  display: grid;
  grid-template-columns: 200px auto 200px;
  gap: 10px;
  align-content: center;

  background: #FFFFFF;
  box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.135216);
  border-radius: 8px;

  padding: 0 10px;
}

.image-product{
  width: 100%;
  padding: 10px 0;
}

.author{
  font-size: .75em;
  color: #7E7E7E;
}

.description{
  font-size: .85em;
  line-height: 20px;
}


.price{
  box-sizing: border-box;
  border-left: 1px solid #DADADA;

  height: 100%;

  display: flex;
  flex-direction: column;

  padding: 10px 0 10px 10px;
}

.price p{
  text-align: center;
  font-size: 1.125em;
}

.classifications{
  background: #787878;
  border-radius: 3px;
  color: #fff;
  width: 55px;
  height: 30px;
  align-self: flex-end;

  text-align: center;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}

.btn{
  display: flex;
  align-items: center;
  justify-content: center;

  padding: 1em .6em;
  font-size: .80em;
  font-weight: 600;
  text-transform: uppercase;

  border-radius: 8px;

  margin: 5px 0;
}

.btn span{
  margin-left: 5px;
}

.heart{
  background: #EDEDED;
}

.buy{
  background: #686868;
  color: #fff;
}


</style>