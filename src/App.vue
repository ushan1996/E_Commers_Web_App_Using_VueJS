<template>
  <v-app>
   <Header></Header>
    <v-main>
      <SliderComponent></SliderComponent>
      <HeaderComponent></HeaderComponent>
      <AboutusComponent></AboutusComponent>
      <PortfolioComponent></PortfolioComponent>
      <ProjectComponent></ProjectComponent>
      <ContactComponent></ContactComponent>
      <FooterComponent> </FooterComponent>
    </v-main>
  </v-app>
</template>

<script>
import Header from "./components/Header-component.vue";
import HeaderComponent from "./components/Body-Component.vue";
import AboutusComponent from "./components/Aboutus-Component.vue";
import PortfolioComponent from "./components/Portfolio-Component.vue";
import ProjectComponent from "./components/Project-Component.vue";
import ContactComponent from "./components/Contact-Component.vue";
import FooterComponent from "./components/Footer-Component.vue";
import SliderComponent from "./components/Slider-Component.vue";


export default {
    name: "App",
    components: { Header, HeaderComponent, AboutusComponent, PortfolioComponent, ProjectComponent, ContactComponent, FooterComponent, SliderComponent }
};
</script>
