<template>
  <div>
    <div v-for="card in cards" :key="card">
      <span>Card: {{ card }} </span>
      <button @click="open(card)">Open</button>
    </div>
    <dialog open v-if="cardSelected">
      CardSelected: {{ cardSelected }}
      <button @click="close">Close</button>
    </dialog>
  </div>
</template>

<script>
export default {
  name: 'app',
  data: () => ({
    cards: [1, 2, 3, 4, 5],
    cardSelected: null,
  }),
  methods: {
    open(item) {
      this.cardSelected = item;
    },
    close() {
      this.cardSelected = null;
    },
  },
};
</script>>

