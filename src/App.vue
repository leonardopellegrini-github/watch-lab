<template>

  <div id="app">

    <HeaderVue/>
    <NuovoJumbo />
    <JumbotronVue />
    <AboutUsVue />
    <BrandVue />
    <ProjectsVue />
    <MagazineVue />
    <FormVue />
    <FooterTopVue />
    <FooterBottomVue />

  </div>

</template>

<script>
import HeaderVue from './components/Header.vue';
import JumbotronVue from './components/Jumbotron.vue';
import AboutUsVue from './components/AboutUs.vue';
import BrandVue from './components/Brand.vue';
import ProjectsVue from './components/Projects.vue';
import MagazineVue from './components/Magazine.vue'
import FormVue from './components/Form.vue';
import FooterTopVue from './components/FooterTop.vue';
import FooterBottomVue from './components/FooterBottom.vue';


export default {
  name: 'App',
  components: {
    HeaderVue,
    JumbotronVue,
    AboutUsVue,
    BrandVue,
    ProjectsVue,
    MagazineVue,
    FormVue,
    FooterTopVue,
    FooterBottomVue,
}
}
</script>

<style lang="scss">

@import url(./assets/_style.scss);

*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  scroll-behavior: smooth;
  scroll-padding-top: 15vh;
}

.margintanto{
  margin-top: 100px
}

.paddingtanto{
  padding: 80px;
}

p, li{
  font-family: "Merriweather";
  padding-bottom: 20px;
}

h1{
  font-family: "Miller";
  font-size: 70px;
  padding-bottom: 20px;
}

@media (max-width:768px) {
  h1{
    font-size: 2.5rem;
  }

  h3{
    font-size: 2rem;
  }
    
}

h3{
  font-family:"Miller";
  font-weight: 400;
  font-size: 50px;
  padding-bottom: 20px;
}

h4{
  font-family:"Montserrat-Regular";
  font-size: 15px;
  padding-bottom: 20px;
}

h5{
  font-family: "Montserrat-Bold";
  font-size: 15px;
  letter-spacing: 4px;
  text-transform: uppercase;
  padding-bottom: 20px;
  
}

button{
  font-family: "Miller";
  font-size: 20px;
  color: #d5c9bc;
  border: 1px solid #d5c9bc;
  background-color: transparent;
  width: 40%;
  margin: auto;
  padding: 10px 20px;
  transition: 0.5s;
  &:hover{
    background-color: #d5c9bc;
    color: white;
    text-decoration: none;
  }
  &:focus{
  outline: none;
  box-shadow: none;
}
}
</style>
