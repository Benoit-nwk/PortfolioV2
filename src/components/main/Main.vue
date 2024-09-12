<script setup>
import Profile from '../images/Profile.vue';
import OpenToWork from '../open_to_work/OpenToWork.vue';
import ButtonDownloadCV from '../buttons/ButtonDownloadCV.vue';
import ButtonContact from '../buttons/ButtonContact.vue';
import Skills from '../skills/Skills.vue';
</script>

<template>
      <main>
            <p>Bonjour, je suis</p><span class="name">Benoît Nowak</span><p>Développeur web junior</p>
            <Profile/>
            <OpenToWork/>
            <div class="sectionButton">
                  <ButtonDownloadCV/>
                  <ButtonContact/>
            </div>
            <Skills/>
      </main>
</template>

<style scoped>
.sectionButton{
      margin: 2rem 0;
      display: flex;
      justify-content: space-around;
      width: 100%;
}

main{
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      margin: 8rem 0;
}

.name{
  font-family: var(--archivoblack);
      font-size: 2rem;
}

</style>
