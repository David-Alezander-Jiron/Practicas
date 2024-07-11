<template>
    <h1></h1>
  </template>
  
  <script>
  export default {
    data() {
      return {
        submenuOpen: false,
      };
    },
    methods: {
      toggleSubMenu() {
        this.submenuOpen = !this.submenuOpen;
      },
    },
  };
  </script>
  
 