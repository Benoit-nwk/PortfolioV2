<script setup>
import ButtonSwitchDarkLightMode from '../buttons/ButtonSwitchDarkLightMode.vue';
</script>

<template>
      <header>
            <ButtonSwitchDarkLightMode/>
      </header>
</template>

<style scoped>
header{
      display: flex;
      justify-content: space-between;
      padding: 1rem;
      background-color: var(--dark);
      box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.1);
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      z-index: 1000;
}
</style>
