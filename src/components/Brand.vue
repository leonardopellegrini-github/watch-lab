<template>

  <div id="brand" class="container margintanto">

    <div class="row d-flex justify-content-center over text-center m-0">
      <div class="col-md-6 colon align-self-center p-5">
        <h5>LONDON COLLECTION SEASON</h5>
        <h3>Temporary Store</h3>
        <p>On the other hand, we denounce with righteous
        indignation and dislike men who are so beguiled and
        demoralized by the charms of pleasure of the moment,
        so blinded by desire</p>
        <button href="Discover">View</button>
      </div>
      <div class="col-md-6 colon align-self-center p-0">
        <img src="../img/bozza-6.jpg" alt="">
      </div>
    </div>

    <div class="row d-flex justify-content-center over text-center m-0">
      <div class="col-md-6 colon align-self-center p-0 order-1">
        <img src="../img/bozza-5.jpg" alt="">
      </div>
      <div class="col-md-6 colon align-self-center order-md-1 p-5">
        <h5>LONDON COLLECTION SEASON</h5>
        <h3>New Selection Of <br> Herny London</h3>
        <p>An estimable experience in the modern collection house</p>
        <button href="Discover">View</button>
      </div>
    </div>

  </div>

</template>

<script>
export default {
name: 'BrandVue'
}
</script>

<style lang="scss" scoped>

#brand{
padding: 0;

  p{
    color:#808080;
  }
  .over{
    height: 100%;
    width: 100%;
  }
  .colon{
    text-align: center;
  }
  .colon img{
 
    width: 100%;
  }
}

</style>