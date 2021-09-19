<template>
  <div class="services">
    <h2 class="title">
      {{ title }}
    </h2>
    <p class="content">
      {{ content }}
    </p>
  </div>
</template>
<script>
import { defineComponent } from "vue";
export default defineComponent({
  props: {
    title: {
      type: String,
      required: true,
    },
    content: {
      type: String,
      required: true,
    },
  },
});
</script>

<style lang="scss" scoped>
.services {
  .title {
    color: #935e92;
    font-weight: bold;
    margin-bottom: 0.8rem;
  }
  .content {
    color: #293947;
    line-height: 1.5;
  }
}
</style>
