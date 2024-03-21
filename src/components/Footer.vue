<script>
  export default {
    
  }
</script>

<template>
  <footer>
    <div class="bottom-bar container d-flex">
      <div class="informazioni">
        <h5>Boolando s.r.l</h5>
        <div>
          <span>Informazioni legali</span>
          <span>Informativa sulla privacy</span>
          <span>Diritto di recesso</span>
        </div>
      </div>
      <div class="social">
        <h6>Trovaci anche su</h6>
        <div>
          <i class="fa-brands fa-square-twitter"></i>
          <i class="fa-brands fa-square-facebook"></i>
          <i class="fa-brands fa-square-instagram"></i>
          <i class="fa-brands fa-square-pinterest"></i>
          <i class="fa-brands fa-youtube"></i>
        </div>
      </div>
  </div>
  </footer>
</template>

<style lang="scss">

footer{
  height: 70px;
  background-color: rgb(26, 26, 26);
  color: white;
  .bottom-bar{
    height: 100%;
    justify-content: space-between;
    align-items: center;
    .informazioni {
      h5{
        font-size: .9rem;
      }
     span{
      font-size: .7em;
      margin-right: 5px;
     }
    }
    .social div{
      margin-top: 8px;
      i{
        margin-right: 10px;
      }
    }
  }
}

</style>