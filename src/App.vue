<template>
  <Nav></Nav>
  <router-view />
 
  
</template>

<script>
import Nav from "@/components/Nav.vue";
export default {
  name: "App",
  components: {
    Nav,
  },
};
</script>

<style lang="scss">


body{
  margin: 0;
  margin-top:0;
  background-color: #eeeeee;
}

@media screen and (min-width: 640px) {
  body{
    margin: 0 30px;
  }
}

@media screen and (max-width: 640px) {
 
}

h1,h2,h3,h4,p{
  margin:0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.sun-grid{
  display: grid;
  grid-template-columns:repeat(12, 1fr);
}

.sun-col-4{
  grid-column:span 4;
}
.sun-col-6{
  grid-column:span 6;
}
.sun-col-8{
  grid-column:span 8;
}
.sun-u-txt--left{
  text-align: left;
}
.sun-u-txt--right{
  text-align: right;
}
.sun-wrapper{
  padding:20px;
}


.sun-label{
  font-size: 14px;
}
.sun-title{
  font-size: 18px;
}
.sun-description{
  font-size: 12px;
}



</style>
