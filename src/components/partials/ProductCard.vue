<script>
export default {
  props: {
    FrontImage: String,
    BackImage: String,
    Name: String,
    Brand: String,
    FullPrice: Number
  }
}
</script>

<template>


  <!-- PRODUCT -->
  <div class="box-product">
    <div class="first-img">
      <img :src="FrontImage" alt="">
    </div>
    <div class="hover-img">
      <img :src="BackImage" alt="">
    </div>
    <div class="marchio"> {{ Brand }} </div>
    <h4>{{ Name }}</h4>
    <div class="price">14,99 € <span>{{ FullPrice }}</span></div>
    <div class="discount">-50%</div>
    <div class="sostenibile">Sostenibilità</div>
    <div class="heart">&hearts;</div>
  </div>


</template>

<style lang="scss">
.box-product .left0 {
  position: relative;
  left: 0;
}

.box-product {
  margin: 0 10px;
  width: 470px;
  /* height: 670px; */
  position: relative;
}

.hover-img {
  position: absolute;
  top: 0;
  display: none;
}

.box-product:hover .hover-img {
  display: block;
}

.box-product:hover .heart {
  color: red;
}

.discount {
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

.sostenibile {
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

.marchio {
  color: rgb(158, 145, 140);
  font-size: .8rem;
}

.price {
  color: red;
  font-size: .8rem;
}

.price span {
  text-decoration: line-through;
  color: black;
}

.heart {
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