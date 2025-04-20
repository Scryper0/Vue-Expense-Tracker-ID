import { defineProps } from 'vue';
<template>
  <div class="inc-exp-container">
    <div>
      <h4>Income</h4>
      <p id="money-plus" class="money plus">
        Rp{{ income.toLocaleString("id-ID") }}
      </p>
    </div>
    <div>
      <h4>Expense</h4>
      <p id="money-plus" class="money minus">
        Rp{{ expenses.toLocaleString("id-ID") }}
      </p>
    </div>
  </div>
</template>

<script setup>
import { defineProps } from "vue";

const props = defineProps({
  income: {
    type: Number,
    required: true,
  },

  expenses: {
    type: Number,
    required: true,
  },
});
</script>
