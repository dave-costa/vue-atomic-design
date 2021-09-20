<template>
  <header class="header">
    <Logo />
    <NavBar class="nav" />
    <Search class="search" />
    <MobileNav class="mb" v-if="active" />
    <button v-if="!active" class="at" @click="active = !active">ativar</button>
    <button v-if="active" class="ats" @click="active = !active">x</button>
  </header>
</template>
<script>
import { defineComponent } from "vue";
import { NavBar, Search } from "@/components/molecules";
import { MobileNav } from "@/components/molecules";
import { Logo } from "@/components/atoms";
export default defineComponent({
  components: {
    NavBar,
    Search,
    Logo,
    MobileNav,
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
.mb {
  display: none;
}
.at {
  display: none;
}
@media (max-width: 720px) {
  .search {
    display: none;
  }
  .nav {
    display: none;
  }
  .mb {
    display: block;
    position: absolute;
    width: 100%;
  }
  .at {
    display: block;
  }
  .ats {
    left: auto;
  }
}
</style>
