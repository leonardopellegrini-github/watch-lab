<template>
  <div id="form" class="container-fluid margintanto formback">
    <div class="row d-flex justify-content-center over text-center vaniglia">

      <div class="col-md-4 colon align-self-center">
        <h3>Get in Touch</h3>
        <h5>DISCOVER MORE ABOUT NEWS,
          EXCLUSIVE EVENTS AND DISCOUNT</h5>
        <div class="input-group">
          
          <input type="email" class="form-control input col-xs-3" placeholder="type your email">
          <span class="input-group-btn">
          <button class="btn" type="submit">OK</button>
          </span>
        </div>
      </div>

    </div>
  </div>
    

</template>

<script>
export default {
  name: 'FormVue'

}
</script>

<style lang="scss" scoped>

.formback{
  color: white;
  background-image: url(../img/bozza-3.jpg);
  background-size: cover;


  .vaniglia{
    background-color: #cabbaacc;
    padding: 40px
  }

  .input, button{
      border: 1px solid white;
      border-radius: 0px;
      background-color: transparent;
      color: white;
      font-family: 'Miller';
      &::placeholder {
      color: white;
      opacity: 1; 
      }
  }

  button{
    margin-left: 15px;
    width: 100%;
  }

}

</style>