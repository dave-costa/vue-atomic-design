<template>
  <nav class="nav-bar">
    <Nav content="Services" link="/services" />
    <Nav content="About me" link="/about" />
    <Nav content="Cases" link="/cases" />
    <Nav content="Contact" link="/contact" />
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
  width: max-content;
  display: grid;
  grid-auto-flow: column;
  grid-gap: 2.5rem;
}
</style>
