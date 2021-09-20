<template>
  <header class="header">
    <Logo />
    <NavBar class="nav" />
    <Search class="search" />
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
  data() {
    return {
      active: false,
    };
  },
});
</script>

<style lang="scss" scoped>
.header {
  width: 100%;
  display: grid;
  grid-template-columns: 160px repeat(3, auto);
  align-items: center;
  justify-content: space-between;
}

@media (max-width: 720px) {
  .search {
    display: none;
  }
  .nav {
    display: none;
  }
}
</style>
