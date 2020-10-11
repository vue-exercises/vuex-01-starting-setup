<template>
  <button @click="addTwo">Add 2</button>
  <button @click="addTen">Add 10</button>
</template>

<script>
export default {
  methods: {
    addTwo() {
      this.$store.dispatch('increment');
    },

    addTen() {
      this.$store.dispatch({
        type: 'increase',
        value: 10
      });
    }
  }
};
</script>
