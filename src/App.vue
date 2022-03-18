
<template>
<div>
 <NavbarComponents />
 <ProdutoFormComponent />
 </div>
</template>

<script>
import NavbarComponents from "./components/NavBar.vue";
import ProdutoFormComponent from "./components/produto/ProdutoForm.vue";

export default {
  name: "App",
  components: {
    NavbarComponents,
    ProdutoFormComponent
    
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
 /* text-align: center;*/
  color: #2c3e50;
  /*margin-top: 60px;*/
}
</style>
