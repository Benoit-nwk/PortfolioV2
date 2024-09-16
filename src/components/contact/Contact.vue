<script>
const sendMail = () => {
      window.open = "mailto:bntnowak@outlook.com"
      }
</script>

<template>
<div>
      <h1>Contactez moi</h1>
      <section id="contact-section">
                  
                  <div class="phone">
                  <h2>Par téléphone</h2>
                  <p>Au: <span>06.58.99.21.89</span></p>
                  <p>Ou en cliquant sur ce bouton:</p>
                  <a href="tel:0658992189">Téléphoner</a>
            </div>
            <div class="mail">
            <h2>Par mail</h2>
            <p>A l'adresse: <span>bntnowak@outlook.com</span></p>
            <p>Ou en cliquant sur ce bouton:</p>
            <a href="mailto:bntnowak@outlook.com">Envoyer un mail</a>
      </div>
        </section>
</div>
</template>



<style scoped>
#contact-section{
      margin: 8rem 0;
      text-align: center;
      animation: fade-in linear;
      animation-timeline: view();
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

}
h1{
      margin: 4rem 0;
      text-align: center;
}

a{
      
      width: 35%;
      height: 4rem;
      color: var(--light);
      font-size: 1.2rem;
      background: transparent;
      border: 0.2rem solid var(--green);
      border-radius: 1rem;
      padding: 0 1rem;
      text-decoration: none;
      display: flex;
      justify-content: center;
      align-items: center;
      margin: 2rem;
}

.phone, .mail{
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
}

@media screen and (min-width: 1080px){
      #contact-section{
            display: grid;
            grid-template-columns: repeat(2, 1fr);
      }
      a{
            width: 50%;
      }
      .phone, .mail{
            margin: 2rem 10rem;
      }
      
}
</style>