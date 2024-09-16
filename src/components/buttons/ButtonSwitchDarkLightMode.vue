<script setup>
import { ref } from 'vue';

const isDarkMode = ref(true);
const lightModeImage='../logos/switch_to_dark_mode.svg';
const darkModeImage= '../logos/switch_to_light_mode.svg';

const darkModeLogo = '../logos/logo_benoit.svg';
const lightModeLogo = '../logos/logo_benoit_light.svg';

const toggleTheme = () => {
  isDarkMode.value = !isDarkMode.value;
  if(isDarkMode.value===false){
    document.body.classList.add('light');
    document.documentElement.classList.add('light');
  } else {
    document.body.classList.remove('light');
    document.documentElement.classList.remove('light');
  }
};

</script>

<template>
            <img :src="isDarkMode ? darkModeLogo : lightModeLogo " alt="logo">
            <button @click="toggleTheme">
                  <img :src="isDarkMode ? darkModeImage : lightModeImage" alt="switch_dark_light" key="theme-image">
            </button>
</template>

<style scoped>
button{
      background-color: transparent;
      border: none;
      padding-right: 1rem;
}

</style>
