<script>
  export default {
    
  }
</script>

<template>
  <header>
    <div>
      <a href="#" class="top-link">Donna</a>
      <a href="#" class="top-link">Uomo</a>
      <a href="#" class="top-link">Bambino</a>
    </div>

    <div>
      <img src="/img/boolean-logo.png" alt="boolean-logo" id="logo">
    </div>

    <div class="icon"> 
      <i class="fa-regular fa-user"></i> <i class="fa-regular fa-heart"></i> <i class="fa-solid fa-bag-shopping"></i> 
    </div>
  </header>
</template>

<style lang="scss">
@use '../assets/scss/partials/variables' as *;

  header{
    height:50px;
    background-color: $bg-header;
    display: flex;
    justify-content: space-around;
    align-items: center;
    color:white;
    font-weight: bold;
    margin-bottom: 20px;
    box-shadow: 0 1px 3px grey;
    width: 100%;
    position: fixed;
    z-index: 999;
      #logo{
        width: 100px;
        height:24px;
        margin-right: 100px;
      }
      .top-link{
        text-decoration: none;
        color: white;
        &:hover{
        text-decoration: underline;
        }
      }
    }
    


</style>