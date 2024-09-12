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
      align-items: center;
      padding:1rem 1rem;
      background-color: var(--color-primary);
      color: var(--color-white);
      box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.1);
}
</style>
