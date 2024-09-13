<script>

</script>

<template>
      <section id="section-about">
            <h2>A propos</h2>
            <div class="about-picture">
                  <img src="../images/about_picture.webp" alt="about-image">
            </div>
            <article>
                  <p>Je m’appelle Benoît j’ai 24 ans et je suis aujourd’hui à la recherche d’un premier job en tant que développeur web.</p>
                  <p>Depuis tout petit je suis passionné par les nouvelles technologies, je commençais déjà à créer quelques petits sites en html & css en classe de 6ème.</p>
                  <p>J’ai décidé après avoir travaillé pendant un peu plus de 2 années en tant que préparateur de commandes, de me réorienter vers le métier de mes rêves : Développeur.</p>
                  <p>J’ai donc suivi une formation chez M2I Formation sur Villeneuve-D'ascq puis j’ai obtenu mon Titre professionnel de Développeur web & web mobile.</p>
            </article>
      </section>
</template>

<style scoped>


#section-about{
      margin: 2rem 0;
      text-align: center;
      animation: in-from-left 1s;
      animation-timeline: view();
}

article{
      margin: 2rem 3rem;
      text-align: center;
}

.about-picture{
      width: 100%;
      display: flex;
      justify-content: center;
      margin: 2rem 0;
      > img{
            width: 60%;
      }
}
</style>