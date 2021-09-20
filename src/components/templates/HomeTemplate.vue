<template>
  <Container class="home">
    <Header class="header" />
    <Presentation class="presentation" />
    <AllServices class="all-s" />
  </Container>
</template>
<script>
import { defineComponent } from "vue";
import { Header, Presentation, AllServices } from "@/components/organisms";
import { Container } from "@/components/matriz/";
export default defineComponent({
  components: {
    Header,
    Presentation,
    AllServices,
    Container,
  },
});
</script>

<style lang="scss" scoped>
.home {
  margin: 5rem auto;
  display: grid;
  grid-gap: 5rem;
}
</style>
