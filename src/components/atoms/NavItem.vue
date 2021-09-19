<template>
  <a class="nav-item" :href="link">
    {{ content }}
  </a>
</template>
<script>
import { defineComponent } from "vue";
export default defineComponent({
  props: {
    content: {
      type: String,
      required: true,
    },
    link: {
      type: String,
      required: true,
    },
  },
});
</script>

<style lang="scss" scoped>
.nav-item {
  color: #293947;
  text-decoration: none;
  font-size: 1.3rem;
}
</style>
