<template>
  <header class="header">
    <Logo />
    <NavBar />
    <Search />
  </header>
</template>
<script>
import { defineComponent } from "vue";
import { NavBar, Search } from "@/components/molecules";
import { Logo } from "@/components/atoms";
export default defineComponent({
  components: {
    NavBar,
    Search,
    Logo,
  },
});
</script>

<style lang="scss" scoped>
.header {
  width: 100%;
  display: grid;
  grid-template-columns: 160px repeat(2, auto);
  align-items: center;
  justify-content: space-between;
}
</style>
