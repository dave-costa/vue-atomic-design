<template>
  <div class="all-s">
    <Services
      title="Front end"
      content="Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae mollitia facere alias nisi accusantium dicta fuga doloremque eos quia ipsam repellat, quisquam, eaque accusamus adipisci libero "
    />
    <Services
      title="Back end"
      content="Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae mollitia facere alias nisi accusantium dicta fuga doloremque eos quia ipsam repellat, quisquam, eaque accusamus adipisci libero "
    />
    <Services
      title="DevOps"
      content="Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae mollitia facere alias nisi accusantium dicta fuga doloremque eos quia ipsam repellat, quisquam, eaque accusamus adipisci libero "
    />
  </div>
</template>
<script>
import { defineComponent } from "vue";
import { Services } from "@/components/molecules/";
export default defineComponent({
  components: {
    Services,
  },
});
</script>

<style lang="scss" scoped>
.all-s {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 5rem;
}
@media (max-width: 720px) {
  .all-s {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    grid-gap: 5rem;
  }
}
</style>
