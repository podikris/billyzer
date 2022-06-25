<template>
  <RecentTransactions limit="3"> </RecentTransactions>
  <CardHolder title="Total spendings"> </CardHolder>
</template>

<script>
import CardHolder from "../components/CardHolder.vue";
import RecentTransactions from "../components/RecentTransactions.vue";

export default {
  name: "Home",
  components: {
    CardHolder,
    RecentTransactions,
  },
};
</script>
