<template>
  <CardHolder title="Recent transactions">
    <div :key="transaction.id" v-for="transaction in transactions">
      <CardTransaction :data="transaction" />
    </div>
  </CardHolder>
</template>

<script>
import CardHolder from "./CardHolder.vue";
import CardTransaction from "./CardTransaction.vue";
export default {
  name: "RecentTransactions",
  components: {
    CardHolder,
    CardTransaction,
  },
  props: {
    limit: Number,
  },
  data() {
    return {
      transactions: [],
    };
  },
  created() {
    this.transactions = [
      {
        id: "1",
        amount: 899,
        date: "2022-06-19",
        purpose: "Clothes",
        mode: "UPI",
        benifits: "Me",
        avoidable: 30,
      },
      {
        id: "2",
        amount: 225,
        date: "2022-06-19",
        purpose: "Home",
        mode: "Cash",
        benifits: "Family",
        avoidable: 0,
      },
      {
        id: "3",
        amount: 899.3,
        date: "2022-06-19",
        purpose: "Clothes",
        mode: "Card",
        benifits: "Daughter",
        avoidable: 50,
      },
    ];
  },
};
</script>
