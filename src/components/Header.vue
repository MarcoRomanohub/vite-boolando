<script>
  export default {
    data(){
      return{
        categories:['Donna', 'Uomo', 'Bambino'],
      }
    }
  }
</script>

<template>
  <header>
    <div class="topbar container d-flex">
      <div class="categorie d-flex">
        <a href="#" class="top-link" v-for="(category, index) in categories" key="index"> {{ category }} </a>
      </div>
      <div class="logo"><img src="/img/boolean-logo.png" alt=""></div>
      <div class="area-personale">
        <i class="fa-regular fa-user"></i>
        <i class="fa-regular fa-heart"></i>
        <i class="fa-sharp fa-solid fa-bag-shopping"></i>        
      </div>
    </div>
  </header>
</template>

<style lang="scss">
@use '../assets/scss/partials/variables' as *;

header{
  height: 50px;
  width: 100%;
  background-color: $bg-header;
  position: fixed;
  z-index: 1;
  .topbar{
    justify-content: space-between;
    align-items: center;
    height: 100%;
  }
  .categorie{
    color: white;
    font-size: .8rem;
    font-weight: bold;
    .top-link{
      text-decoration: none;
      color: white;
      margin: 0 8px;
      &:hover{
        text-decoration: underline;
      }
    }
  }
  .logo{
    width: 100px;
  }
  .area-personale{
    font-size: .8rem;
    color: white;
    i{
      padding-right: 5px;
    }
  }
}


</style>