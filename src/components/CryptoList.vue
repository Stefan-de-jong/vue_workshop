<template>
  <table class="table">
    <thead>
      <td>Name</td>
      <td>Price</td>
    </thead>
    <tbody v-for="crypto in currencies" :key="crypto.name">
      <tr>
        <td>{{ crypto.name }}</td>
        <td>{{ crypto.price }}</td>
      </tr>
    </tbody>
    <button @click="changeValue()">Click meeeeeeee</button>
  </table>
</template>

<script>
export default {
  name: "CryptoList",
  data() {
    return {
      currencies: [
        { name: "Bitcoin", price: 9000 },
        { name: "Ethereum", price: 6541 },
        { name: "Dogecoin", price: 1242 },
        { name: "Chainlink", price: 7568 },
        { name: "Ripple", price: 1783 },
      ],
    };
  },
  methods: {
    changeValue() {},
  },
};
</script>

<style>
</style>