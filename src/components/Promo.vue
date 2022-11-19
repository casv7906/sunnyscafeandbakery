<template>
  <div class="sun-promo sun-grid">
    <img class="sun-promo__img sun-col-6" src="@/assets/promo1.jpg" alt=""/>
    <div class="sun-wrapper sun-col-6 sun-promo__text">
      <h3>{{ label }}</h3>
      <h4>{{ title }}</h4>
      <p>{{ description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Promo",
  props: ["label", "title", "description"],
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
.sun-promo{
  background-color: #e0e0e0;
  border-radius: 5px;
  position: relative;
}
.sun-promo__img{
  border-radius: 5px;
  position: relative;
  width: 100%;
}
</style>
