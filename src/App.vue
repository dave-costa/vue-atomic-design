<template>
  <HomeTemplate />
</template>

<script>
import { defineComponent } from "vue";
import { HomeTemplate } from "@/components/templates";
export default defineComponent({
  name: "App",
  components: {
    HomeTemplate,
  },
});
</script>
<style lang="scss" scoped></style>
