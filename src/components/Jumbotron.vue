<template>

  <div class="contenitore">
    
    <div class="text">
    <h5>LONDON COLLECTION SEASON</h5>
    <h1>New Selection Of <br> Herny London</h1>
    <h4>An estimable experience in the modern collection house</h4>
    <button onclick="location.href='#aboutus'"> Discover </button>
  </div>
  <div class="post">
    <div class="dentrotesto">
      <h6>The Path to Success with Watchlab</h6>
      <p href="#">NEXT ></p>
    </div>
  </div>

  </div>
    
</template>

<script>
export default {
  name: 'JumbotronVue'
}
</script>

<style lang="scss" scoped>

.contenitore{
  background-image: url(../img/bozza-4.jpg);
  background-position: center;
  background-size: cover;
  position: relative;

  
  .text{
    width: 100%;
    background-color: rgba(0, 0, 0, 0.444);
    height: 100%;
    min-height: 600px;
    color: white;
    display: flex;
    text-align: center;
    justify-content: space-evenly;
    flex-direction: column;
    padding: 40px;
    margin: auto;
    a{
      width: 100%;
    }
    h1, h5, h4{
      width: 40%;
      padding-bottom: 20px;
      margin: auto;
    }
  }

  .post{
    display: block;
    width: 300px;
    height: 200px;
    position: absolute;
    z-index: 2;
    bottom: 0;
    right: 0;
    background-image: url(../img/bozza-8.jpg);
    background-position: center;
    background-size: cover;
    margin-right: 10%;
    transition: ease 0.5s;
    .dentrotesto{
      color: white;
      background-color: rgba(0, 0, 0, 0.564);
      height: 100%;
      width: 100%;
      position: absolute;
      z-index: 3;
      transition: ease 0.5s;
      h6{
        top: 0;
        left: 0;
        position: absolute;
        font-size: 20px;
        font-family: "Miller";
        padding: 10px;
        width: 70%;
      }
      button{
        width: 25%;
      }
      p{
        bottom: 0;
        right: 0;
        position: absolute;
        padding: 10px;
        font-family: "Montserrat-Bold";
        font-weight: 300;
        letter-spacing: 4px;
        transition: ease 0.5s;
      }
      p:hover{
        letter-spacing: 2px;
      }
      &:hover{
        background-color: rgba(0, 0, 0, 0.162);
    }
    }
   
  }
  @media (max-width: 1250px) {
      .post{
        display: none;
      }
    }
}

@media (max-width: 400px) {
    .contenitore .text h1, .contenitore .text h5, .contenitore .text h4 {
     width: 90%;
     padding-bottom: 20px;
     margin: 20px auto;
     }
}

</style>