<script>

</script>


<template>
      <h1>Mes Réalisations</h1>
      <section id="section-project">
            
            <div class="project">

                        <h2>Portfolio</h2>
                        <p>Projet réalisé post formation. Il contient ma biographie, mes Skills, mes coordonnées ainsi que une présentation de mes projets.</p>
                        <a href="https://github.com/Benoit-nwk/Portfolio"><img src="../icons/github_W.svg" alt="logo_github"></a>
            </div>
            <div class="project">
                        <h2>Kayu</h2>
                        <p>Projet réalisé durant la formation. Il s'agit d'une reproduction d'application nommée 'Yuka', elle présente une partie frontend et une partie backend. Ce projet est composé d'un CRUD (create, read, update, delete). Il est possible de scanner un article qui fait un appel API pour collecter les informations du produit❗Projet Mobile uniquement❗</p>
                        <a href="https://github.com/Benoit-nwk/Kayu"><img src="../icons/github_W.svg" alt="logo_github"></a>
            </div>
            <div class="project">

                        <h2>AnthonyM.Coiffure</h2>
                        <p>Projet réalisé durant le stage de formation. Il s'agit ici d'une refonte du site internet vitrine d'un salon de coiffure. Le site est composé de plusieurs pages, il est possible de consulter les tarifs et de voir les horaires d'ouverture.</p>
                        <a href="https://github.com/Benoit-nwk/Anthony-M-Coiffure"><img src="../icons/github_W.svg" alt="logo_github"></a>
            </div>
            <div class="project">

                        <h2>Calculator 3000</h2>
                        <p>Projet réalisé durant la formation. Ici, le but était de réaliser une calculatrice en utilisant les bases de Vue.js. La calculatrice est fonctionnelle et permet de réaliser des opérations simples.</p>
                        <a href="https://github.com/Benoit-nwk/Calculator3000"><img src="../icons/github_W.svg" alt="logo_github"></a>
            </div>
      </section>
</template>


<style scoped>
h1{
      text-align: center;
      margin: 4rem 0;
}

#section-project{
      margin: 8rem 0;
      text-align: center;
}
.project{
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      margin: 2rem 2rem;
      padding: 1rem;
      border: 0.2rem solid var(--green);
      border-radius: 5px;
      background-color: var(--primary-color);
      animation: fade-in 1s;
      animation-timeline: view(); 
}

@media screen and (min-width: 1080px){
      #section-project{
            display: grid;
            grid-template-columns: repeat(2, 1fr);
      }
      .project{
            margin: 2rem 10rem;
      }
      
}
</style>