<template>
  <div class="home">
    <div class="icons" v-on:mouseover="hoverMenu = true" v-on:mouseout="hoverMenu = false">
      <img v-if="!hoverMenu"  title="Menu" id="menu-icon" src="../assets/help_outline_24px.svg" alt="menu bar">
      <img v-else-if="hoverMenu"  title="Menu" id="menu-icon" src="../assets/help_24px.svg" alt="menu bar">

    </div>
  </div>
</template>

<script>

export default {
  data: function() {
        return {
            hoverMenu: null
        }
    },
};
</script>

<style scoped>
  .icons {
    background: #f1f1f1;
  }
</style>