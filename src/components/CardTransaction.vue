<template>
  <div class="avoidable"></div>
  <div class="left-panel">
    <span class="amount">{{ data.amount }}</span>
    <span class="date">{{ data.date }}</span>
  </div>
  <div class="right-panel">
    <span class="purpose">{{ data.purpose }}</span>
    <span class="payment-mode">{{ data.mode }}</span>
    <span class="beneficiary">{{ data.benefits }}</span>
  </div>
</template>

<script>
export default {
  name: "CardTransaction",
  props: {
    data: Object,
  },
};
</script>
