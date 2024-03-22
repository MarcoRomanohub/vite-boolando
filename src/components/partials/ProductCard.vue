<script>
  export default {
    
  }
</script>

<template>
  
  <div class="container d-flex">
      <!-- PRIMO PRODOTTO -->
      <div class="box-product">
        <div class="first-img">
          <img src="/public/img/1.webp" alt="">
        </div>
        <div class="hover-img">
          <img src="/public/img/1b.webp" alt="">
        </div>
        <div class="marchio">Levi's</div>
        <h4>RELAXED FIT TEE UNISEX</h4>
        <div class="price">14,99 € <span>29,99 €</span></div>
        <div class="discount">-50%</div>
        <div class="sostenibile">Sostenibilità</div>
        <div class="heart">&hearts;</div>
      </div>
      <!-- SECONDO PRODOTTO -->
      <div class="box-product">
        <div class="first-img">
          <img src="/public/img/2.webp" alt="">
        </div>
        <div class="hover-img">
          <img src="/public/img/2b.webp" alt="">
        </div>
        <span class="marchio">Guess</span>
        <h4>ROSES TEE</h4>
        <div class="price">20,99 € <span>29,99 €</span></div>
        <div class="discount">-30%</div>
        <div class="heart">&hearts;</div>
      </div>
      <!-- TERZO PRODOTTO -->
      <div class="box-product">
        <div class="first-img">
          <img src="/public/img/3.webp" alt="">
        </div>
        <div class="hover-img">
          <img src="/public/img/3b.webp" alt="">
        </div>
        <span class="marchio">Come Zucchero Filato</span>
        <h4>VOGLIA DI COLORI PASTELLO</h4>
        <div class="price">129,99 € <span>184,99 €</span></div>
        <div class="discount">-30%</div>
        <div class="heart">&hearts;</div>
      </div>
    </div>
    <div class="container d-flex">
      <!-- QUARTO PRODOTTO -->
      <div class="box-product">
        <div class="first-img">
          <img src="/public/img/4.webp" alt="">
        </div>
        <div class="hover-img">
          <img src="/public/img/4b.webp" alt="">
        </div>
        <div class="marchio">Levi's</div>
        <h4>TEE UNISEX</h4>
        <div class="price">14,99 € <span>29,99 €</span></div>
        <div class="discount">-50%</div>
        <div class="sostenibile">Sostenibilità</div>
        <div class="heart">&hearts;</div>
      </div>
      <!-- QUINTO PRODOTTO -->
      <div class="box-product">
        <div class="first-img">
          <img src="/public/img/5.webp" alt="">
        </div>
        <div class="hover-img">
          <img src="/public/img/5b.webp" alt="">
        </div>
        <span class="marchio">Maya Deluxe</span>
        <h4>STRIPE BODICE</h4>
        <div class="price">99,99 €</div>
        <div class="heart">&hearts;</div>
      </div>
      <!-- SESTO PRODOTTO -->
      <div class="box-product">
        <div class="first-img">
          <img src="/public/img/6.webp" alt="">
        </div>
        <div class="hover-img">
          <img src="/public/img/6b.webp" alt="">
        </div>
        <span class="marchio">Esprit</span>
        <h4>MAGLIONE - BLACK</h4>
        <div class="price">129,99 €</div>
        <div class="sostenibile left0">Sostenibilità</div>
        <div class="heart">&hearts;</div>
      </div>
    </div>

</template>

<style lang="scss">


.box-product .left0{
  position: relative;
  left: 0;
}
.box-product{
  margin: 0 10px;
  width: 470px;
  /* height: 670px; */
  position: relative;
}
.hover-img{
  position: absolute;
  top: 0;
  display: none;
}
.box-product:hover .hover-img{
display: block;
}
.box-product:hover .heart{
  color: red;
}
.discount{
  background-color: red;
  width: 40px;
  height: 20px;
  text-align: center;
  line-height: 20px;
  position: relative;
  bottom: 120px;
  color: white;
  font-size: .7rem;
  font-weight: bold;
}
.sostenibile{
  background-color: green;
  width: 90px;
  height: 20px;
  font-size: .7rem;
  text-align: center;
  line-height: 20px;
  position: relative;
  bottom: 140px;
  left: 43px;
  color: white;
  font-weight: bold;
}
.marchio{
  color: rgb(158, 145, 140);
  font-size: .8rem;
}
.price{
  color: red;
  font-size: .8rem;
}
.price span{
  text-decoration: line-through;
  color: black;
}
.heart{
  background-color: white;
  width: 50px;
  height: 50px;
  text-align: center;
  line-height: 50px;
  font-size: 25px;
  position: absolute;
  top: 10px;
  right: 0;
}

</style>
