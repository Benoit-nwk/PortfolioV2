<script setup>
const downloadCV = () => {
      window.open("../public/CV_Nowak_Benoit.pdf")
}
</script>

<template>
<button @click="downloadCV"  class="button_main">Télécharger mon cv</button>
</template>

<style scoped>

</style>
