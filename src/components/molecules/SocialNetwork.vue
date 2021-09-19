<template>
  <div class="social-network">
    <Link to="https://facebook.com" name="facebook" icon="facebook" />
    <Link to="https://github.com/dave-costa" name="github" icon="github" />
    <Link to="https://twitter.com" name="twitter" icon="twitter" />
  </div>
</template>
<script>
import { defineComponent } from "vue";
import { Link } from "@/components/atoms";
export default defineComponent({
  components: {
    Link,
  },
});
</script>

<style lang="scss" scoped>
.social-network {
  display: grid;
  grid-gap: 1rem;
}
</style>
