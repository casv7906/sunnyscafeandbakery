<template>
  <router-link to="/" class="sun-logo">
    <img class="sun-logo__img" src="@/assets/logo.png" alt="Sunny's cafe and bakery" />
  </router-link>
</template>

<script>
export default {
  name: "Logo",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
.sun-logo{
  width: 100px;
  height: 40px;
  display: inline-block;
}
.sun-logo__img{
  border-radius: 5px;
    height: 100%;
    object-fit: cover;
    vertical-align: bottom;
}

@media screen and (min-width: 640px) {
  .sun-logo{
  width: 200px;
  height: 60px;
}

}


</style>
