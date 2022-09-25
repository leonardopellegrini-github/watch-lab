<template>
  <div id="contacts" class="container-fluid foottop paddingtanto">
    <div class="row">
      <img src="../img/logo-wlab.png" alt="Logo">
    </div>
    <div class="row">
      <div class="col-12 col-md-2">
        <ul>
          <li>Watch/Lab Innovation brings success</li>
          <li>Via Borgogna 5, Milan</li>
          <li>Italy</li>
        </ul>
      </div>
      <div class="col-12 col-md-2">
        <ul>
          <li>About us</li>
          <li>Brand</li>
          <li>Projects</li>
          <li>Magazine</li>
        </ul>
      </div>
      <div class="col-12 col-md-2">
        <ul>
          <li>Press</li>
          <li>Contacts</li>
          <li>Privacy Policy</li>
          <li>Search</li>
        </ul>
      </div>
      <div class="col-12 col-md-2">
        <ul>
          <li>T. +39 392 9133937</li>
          <li>M. info@watch-lab.it</li>
          <li>FACEBOOK</li>
          <li>INSTAGRAM</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:'FooterTopVue',
}
</script>

<style lang="scss" scoped>

.foottop{
  background-color: #333;
  color: #d0c5b6;
  img{
    margin-bottom: 40px;
  }
  ul{
    list-style: none;
    li{
      padding-bottom: 20px;
      font-size: 15px;
    }
  }
}

@media (max-width:450px){
  .paddingtanto{
  padding: 20px;
  }
  img{
    width: 100%;
  }
}

</style>