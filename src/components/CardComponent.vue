<template>
  <div>
    <h2>{{ cardTitle }}</h2>
    <p>Card number one</p>
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: "CardComponent",
  props: ['cardTitle']
}
</script>

<style scoped>
div {
  border: 1px solid black;
  box-shadow: 1px 1px 2px #2c3e50;
  width: 100%;
  padding: 30px;
  margin: auto;
  text-align: center;
}
</style>