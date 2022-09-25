<template>
   <div id="projects" class="container duecolor margintanto">
    <div class="row">
      <div class="col p-0">
        <h3>Press from
        Watch Lab Studio</h3>
      </div>
    </div>
    <div class="row">

      <div class="col-md-4 m-0 p-0">
        <p>{{ sliderImages[contaImm].description }} </p>
      </div>

      <div class="col-md-4 m-0 p-0 contenitoreImmagine">
        <img :src="require('../img/'+ sliderImages[contaImm].image)" :alt="sliderImages[contaImm].category">
      </div>

      <div class="col-md-4 m-0 pl-3 informazioni">
        <h5>{{ sliderImages[contaImm].category }}</h5>
        <h5 class="data">{{ sliderImages[contaImm].data }}</h5>
        <h3>{{ sliderImages[contaImm].title }}</h3>
        <i @click="avanti()" class="fa-solid fa-chevron-left"></i>
        <i @click="indietro()" class="fa-solid fa-chevron-right"></i>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name:'ProjectsVue',
  data(){
    return{
      sliderImages: [
        {
            image: 'bozza-7.jpg',
            category: 'PRESS',
            data:  '18 SETTEMBRE 2015',
            title: 'Most Important Days on Watchlab',
            description: 'On the other hand, we denounce with righteous indignation and dislike men who are so beguiled and demoralized  by the charms of pleasure of the moment, so blinded by desire, that they cannot foresee the pain trouble',
        },
        {
            image: 'bozza-6.jpg',
            category: 'PRESS',
            data:  '20 OTTOBRE 2018',
            title: 'Most Important Days on Watchlab',
            description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Numquam molestias esse illum quibusdam velit dolorem a, ipsam quae atque obcaecati itaque id. Neque omnis ullam doloremque laboriosam dolorem laborum cupiditate. Porro magni non corrupti veritatis aperiam vitae eligendi magnam? Quaerat saepe asperiores, facilis repellendus pariatur blanditiis deleniti quisquam consequuntur in.',
        },
        {
            image: 'bozza-5.jpg',
            category: 'PRESS',
            data:  '15 FEBRRAIO 2019',
            title: 'Most Important Days on Watchlab',
            description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Numquam molestias esse illum quibusdam velit dolorem a, ipsam quae atque obcaecati itaque id.',
        }
      ],
      contaImm: 0,
    }
  },
  methods:{
    avanti(){
      this.contaImm++;
      if(this.contaImm > this.sliderImages.length - 1){
      this.contaImm = 0;
      }
    },
    indietro(){
      this.contaImm--;
      if (this.contaImm < 0){
      this.contaImm = this.sliderImages.length - 1;
      }     
    },
  },
}
</script>

<style lang="scss" scoped>

.duecolor{
  background: linear-gradient(to left, #EFEFEF 50%, #fff 50%);
  padding: 30px;

  p{
      color:#808080;
  }

  @media (max-width:700px){
    p{
      height: 200px;
    }
  }

  .contenitoreImmagine{
    width: 350px;
    height: 350px;
    overflow:hidden;
    object-fit: cover;
    img{
    height: 100%;
    width: 100%;
    padding-bottom: 15px;
    }
  }
  
  .informazioni {
    .data{
    color:#d5c9bc;
    }
    h5{
      padding-bottom: 0;
    }
    h3{
      font-size: 25px;
      padding-top: 10px
    }
    i{
      margin-right: 10px;
      transition: ease 0.5s;
      border: none;
      padding: 5px;
      &:hover{
        color: white;
        border-radius: 50px;
        background-color: #C5B3A1;
      }
    }

  }

}

</style>