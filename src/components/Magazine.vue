<template>
  <div id="magazine" class="container dimensiongrid mt-5">
    <div class="row">
      <div class="col-sm-6 p-0 ml">
         <img src="../img/bozza-11.jpg" alt="Imm">
        <div class="testo">
          <h5>Instagram</h5>
          <h3>Discover Watch Lab</h3>
        </div>
      </div>
      <div class="col-sm-6 p-0 d-flex flex-wrap">
        <div class="sl">
            <img src="../img/bozza-9.jpg" alt="Imm">
            <div class="testo">
              <h5>Instagram</h5>
              <h3>Discover Watch Lab</h3>
            </div>
          </div>
          <div class="sl">
            <img src="../img/bozza-13.jpg" alt="Imm">
            <div class="testo">
              <h5>Instagram</h5>
              <h3>Discover Watch Lab</h3>
            </div>
          </div>
          <div class="sl">
            <img src="../img/bozza-12.jpg" alt="Imm">
            <div class="testo">
              <h5>Instagram</h5>
              <h3>Discover Watch Lab</h3>
            </div>
          </div>
          <div class="sl">
            <img src="../img/bozza-10.jpg" alt="Imm">
            <div class="testo">
              <h5>Instagram</h5>
              <h3>Discover Watch Lab</h3>
            </div>
          </div>
      </div>
    </div>
    
    

  </div>
</template>

<script>
export default {
  name: 'MagazineVue',
}
</script>

<style lang="scss" scoped>

#magazine{
  img{
    width: 100%;
  }

  h3{
    text-align: center;
    padding-top: 10%;
    font-size: 30px;
  }

  .sl{
    width: 50%;
    position: relative;
    transition: all 1s ease;
  }

  .ml{
    transition: all 1s ease;
  }

  .testo{
    display: none;
    background-color: rgba(0, 0, 0, 0);
    transition: all 1s ease;
  }

  .ml:hover > div, .sl:hover > div {
    display: flex;
    color: white;
    background-color: rgba(0, 0, 0, 0.564);
    height: 100%;
    width: 100%;
    position: absolute;
    z-index: 3;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }
}



</style>