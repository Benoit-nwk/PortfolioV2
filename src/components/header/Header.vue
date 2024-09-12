<script setup>
import { ref } from 'vue';

const isDarkMode = ref(true);
const lightModeImage='../logos/switch_to_dark_mode.svg';
const darkModeImage= '../logos/switch_to_light_mode.svg';


const toggleTheme = () => {
  isDarkMode.value = !isDarkMode.value;
  if(isDarkMode.value===false){
    document.documentElement.classList.add('light');
  } else {
    document.documentElement.classList.remove('light');
  }
};
</script>

<template>
      <header>
            <a href=""><img src="../logos/logo_benoit.svg" alt="logo_benoit"></a>
            <button @click="toggleTheme">
                  <img :src="isDarkMode ? darkModeImage : lightModeImage" alt="switch_dark_light" key="theme-image">
            </button>
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

button{
      background-color: transparent;
      border: none;
}
</style>
