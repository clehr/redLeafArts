<template>
  <div class="columns is-multiline">
    <PaintingCard />
    <PaintingCard />
    <PaintingCard />
    <PaintingCard />
    <PaintingCard />
    <PaintingCard />
    <PaintingCard />
    <PaintingCard />
    <PaintingCard />
    <PaintingCard />
  </div>
</template>

<script>
import PaintingCard from "~/components/PaintingCard.vue";

export default {
  components: {
    PaintingCard
  }
};
</script>

<style scoped>
.columns {
  margin-left: 15%;
}
</style>
