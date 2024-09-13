<script setup>
import Profile from '../images/Profile.vue';
import OpenToWork from '../open_to_work/OpenToWork.vue';
import ButtonDownloadCV from '../buttons/ButtonDownloadCV.vue';
import ButtonContact from '../buttons/ButtonContact.vue';
import About from '../about/About.vue';
import Projects from '../projects/Projects.vue';
import Contact from '../contact/Contact.vue';
const skillsTab = ["VsCode", "PhpStorm", "HTML", "CSS", "JavaScript", "PHP", "Vue.Js", "Laravel", "MySql", "Laragon", "Git", "Figma"]

</script>

<template>
      <main>

<!--Section de bienvenue-->
            <section id="section-hello">
                  <p>Bonjour, je suis</p>
                  <span class="name">Benoît Nowak</span>
                  <p>Développeur web junior</p>
                  <Profile/>
                  <OpenToWork/>

<!--Alignement des boutons-->
                  <div class="align-button">
                        <ButtonDownloadCV/>
                        <ButtonContact/>
                  </div>
            </section>

<section id="section-skills">
      <h2>Mes compétences</h2>
            <div class="tab-of-skills">
                  <div class="skills" v-for="skills in skillsTab">
                        <span>{{ skills }}</span>
                  </div>
            </div>
</section>
      <About/>
      <Projects/>
      <Contact/>
      </main>
</template>

<style scoped>



#section-hello{
      text-align: center;

}

#section-skills{
      margin: 5rem 2rem;
      text-align: center;
      animation: fade-in linear;
      animation-timeline: view();
}

.align-button{
      margin: 2rem 0;
      display: flex;
      justify-content: space-around;
      width: 100%;
}

main{
      margin: 8rem 0;
}

.name{
      font-family: var(--archivoblack);
      font-size: 2rem;
}



.tab-of-skills{
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      gap: 1rem;
}

.skills{
      display: flex;
      justify-content: center;
      align-items: center;
      border: 0.3rem solid var(--grey);
      padding: 1rem;
      border-radius: 0.5rem;
}
</style>
