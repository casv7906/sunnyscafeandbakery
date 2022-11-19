<template>
  <div class="home">
    <Hero title="Title" label="Label" description="description"/>
    <Promo title="Title" label="Label" description="description"/>
  </div>
</template>

<script>
import Hero from "@/components/Hero.vue";
import Promo from "@/components/Promo.vue";
export default {
  name: "Home",
  components: {
    Hero,
    Promo,

  },
};
</script>
