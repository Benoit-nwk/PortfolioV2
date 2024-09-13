<script>
const sendMail = () => {
        window.location.href = "mailto:bntnowak@outlook.com"
}

const call = () => {
        window.location.href = "tel:0658992189"
}

</script>

<template>
<div>
      <section id="contact-section">
            <h1>Contactez moi</h1>

            <h2>Par téléphone</h2>
            <p>Au: <span>06.58.99.21.89</span></p>
            <p>Ou en cliquant sur ce bouton:</p>
            <button @click="call">Apeller</button>
            <h2>Par mail</h2>
            <p>A l'adresse: <span>bntnowak@outlook.com</span></p>
            <p>Ou en cliquant sur ce bouton:</p>
            <button @click="sendMail">Contacter par mail</button>
        </section>
</div>
</template>



<style scoped>
#contact-section{
      margin: 8rem 0;
      text-align: center;
      animation: fade-in linear;
      animation-timeline: view();
}
h1{
      margin: 4rem 0;
}
button{
      width: 35%;
  height: 4rem;
  color: var(--light);
  font-size: 1.2rem;
  background: transparent;
  border: 0.2rem solid var(--green);
  border-radius: 1rem;
  padding: 0.5rem 1rem;
}
</style>