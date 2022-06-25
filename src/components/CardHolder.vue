<template>
  <div class="card-holder">
    <span class="title">{{ title }}</span>
    <slot></slot>
  </div>
</template>

<script>
import CardTransaction from "../components/CardTransaction.vue";
export default {
  name: "CardHolder",
  components: {
    CardTransaction,
  },
  props: {
    title: String,
  },
};
</script>

<style scoped>
.title {
  color: darkgray;
}
</style>
