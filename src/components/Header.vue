<template>

<nav id="header" class="navbar navbar-expand-lg navbar-light p-0">
  <a class="navbar-brand backlogo" href="#"><img src="../img/logo-wlab.png" alt="Logo"></a>
  <button id="nobordo" class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div  class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item nuovolink" :key="`menu-${index}`" v-for="(menu, index) in menus">
        <a class="nav-link nuovolink" :href="menu.link">{{menu.title}}</a>
      </li>
      
    </ul>
    <form class="form-inline my-2 my-lg-0 p-3">
      <input class="form-control input-sm" id="inputsm" type="text">
      <button class="btn btn-outline-success my-2 my-sm-0" type="submit"><i class="fa-solid fa-magnifying-glass"></i>
      </button>
    </form>
  </div>
  </nav>
  
</template>

<script>
export default {
  name: 'HeaderVue',
  data(){
    return{
      menus: [
        {
            title: 'About us',
            link: '#aboutus',
        },
        {
            title: 'Brand',
            link: '#brand',
        },
        {
            title: 'Projects',
            link: '#projects',
        },
        {
            title: 'Magazine',
            link: '#magazine',
        },
        {
            title: 'Press',
            link: '#form',
        },
        {
            title: 'Contacts',
            link: '#contacts',
        },
       
      ],
    }
  }
}
</script>

<style lang="scss" scoped>

#header{
  position: sticky;
  top:0;
  background: white;
  z-index: 5;

  .nuovolink{
  border: none;
  color: black;
  font-family: 'Montserrat-regular';
  font-size: 15px;
  padding: 8px 20px; 
}

.navbar-nav,
.mr-auto {
flex: 1;
margin: auto !important;
display: flex;
justify-content: space-between;
}

.backlogo{
  background-color: #d5c9bc;
  margin: 0;
  img{
    width: 100%;
    padding: 10px;
  }
}

.new{
  border: none;
  color: black;
  background: none;
  font-family: 'Montserrat';
  font-weight: 500;
  font-size: 15px;
  margin-left: 20px;
}

input, button{
  color: black;
  border: none;
  border-radius: 0;
  padding: 0;
}

input{
  border-bottom: 2px solid black;
  width: 50%;
}

button:hover{
  background-color: transparent;
}

}

@media (max-width:450px) {
  #header{
    .backlogo{
    width: 60%;
    padding: 0px;
    img{
    width: 100%;
    padding: 10px;
    }
   }
  }
  
    
}

</style>