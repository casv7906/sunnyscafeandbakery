<template>
  <nav class="sun-nav sun-grid">
    <div class="sun-col-4 sun-u-txt--left">
      <Logo />
    </div>
    <div class="sun-col-8 sun-u-txt--right">
      <router-link to="/" class="sun-nav__link">Home</router-link>
      <router-link to="/menu" class="sun-nav__link">Menu</router-link>
    </div>
  </nav>
</template>

<script>
import Logo from "@/components/Logo.vue";
export default {
  name: "Nav",
  components: { Logo },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
.sun-nav {
    background:linear-gradient(180deg, rgba(62,62,62,1) 50%, rgba(58,58,58,1) 100%);
    border-radius: 5px;
    align-items: center;
    padding-right:20px;
    position: relative;
    z-index: 1000;}
  .sun-nav__link {
    font-size:12px;
    font-weight: bold;
    color: #ffffff;
    padding:0 5px;
    text-decoration: none;
    &:hover{
        color: #3f9691;  
    }

    &.router-link-exact-active {
      color: #3f9691;
      text-decoration: underline;
    }
  }


@media screen and (min-width: 640px) {
    .sun-nav__link {
    font-size:16px;
    padding:0 10px;
}

}
</style>
