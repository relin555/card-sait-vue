<template>
  <button class="button">
    <slot></slot>
  </button>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
  .button {
    background: linear-gradient(87.32deg, #E2A300 4.47%, #E29500 95.53%);
    box-shadow: 0px 2px 13px rgba(226, 158, 0, 0.48);
    border-radius: 6px;
    padding: 14px 38px 13px 41px;
    font-weight: 600;
    font-size: 18px;
    line-height: 20px;
    color: #000000;
    outline: none;
    border: none;
    text-transform: uppercase;
  }
</style>