<template>
    <button class="btn">
      {{ title }}
    </button>
  </template>
  
  <script lang="ts">
  export default {
    props: {
      title: {
        type: String as PropType<string>,
        required: true,
      },
    },
  };
  </script>
  
  <style lang="scss" scoped>
  .btn {
    min-width: 200px;
    padding: 12px;
    border: solid 2px;
    border-color: rgb(1, 204, 1);
    box-shadow: rgb(0, 120, 14) 2px 7px 14px;
    color: rgb(255, 255, 255);
    text-transform: uppercase;
    font-weight: 600;
    background-color: rgb(0, 0, 0);
    cursor: pointer;
  
    transition: 0.05s;
  
    &:hover {
      background: black;
      color: white;
      transform: translate(-4px, -4px);
    }
  }
  </style>
  