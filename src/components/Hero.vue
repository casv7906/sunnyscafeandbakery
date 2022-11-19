<template>
  <div class="sun-hero sun-grid">
    <div class="sun-wrapper sun-col-6 sun-hero__text">
      <h2 class="sun-label">{{ label }}</h2>
      <h1 class="sun-title">{{ title }}</h1>
      <p class="sun-desc">{{ description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Hero",
  props: ["label", "title", "description"],
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
.sun-hero{
  position: relative;
  border-radius: 5px;
  min-height: 200px;
  background:linear-gradient(180deg, rgba(0,0,0,0.4) 50%, rgba(0,0,0,1) 100%),url('~@/assets/hero1.jpg');
  background-size: cover;
  align-items: center;

}

.sun-hero__text{
  color:#fff;
  grid-column:span 12;
  text-align: center;
}


@media screen and (min-width: 640px) {
  .sun-hero{
    min-height: 300px;
  }

.sun-hero__text{
  grid-column:span 6;
  text-align: left;
}
}


</style>
