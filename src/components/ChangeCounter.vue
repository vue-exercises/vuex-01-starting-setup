<template>
  <button @click="addTwo">Add 2</button>
  <button @click="addTen">Add 10</button>
</template>

<script>
export default {
  methods: {
    addTwo() {
      this.$store.commit('increment');
    },

    addTen() {
      // this.$store.commit('increase', { value: 10 });
      this.$store.commit({
        type: 'increase',
        value: 10
      });
    }
  }
};
</script>
