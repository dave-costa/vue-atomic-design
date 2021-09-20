<template>
  <nav class="nav-bar">
    <Nav class="services" content="Services" link="/services" />
    <Nav class="about" content="About me" link="/about" />
    <Nav class="cases" content="Cases" link="/cases" />
    <Nav class="contact" content="Contact" link="/contact" />
  </nav>
</template>
<script>
import { defineComponent } from "vue";
import { Nav } from "@/components/atoms";
export default defineComponent({
  components: {
    Nav,
  },
});
</script>

<style lang="scss" scoped>
.nav-bar {
  width: 100%;
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
}
</style>
