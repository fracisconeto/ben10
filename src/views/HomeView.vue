<script setup>
import { RouterLink } from 'vue-router'

</script>

<template>
  <section class="series-ben10">
        <div class="container-fundo">
          <img src="../assets/img/classico/fundo.webp" alt="" />
        </div>
        <h2>É hora do herói!</h2>

        <div class="serie">
         
          <p>
            Descubra todos os alienígenas do Omnitrix e mergulhe no universo do Ben 10 clássico.

          </p>
          <RouterLink to="/alienigenas" class="btn-link">Ver Alienígenas</RouterLink>
          <RouterLink to="/personagens" class="btn-link">Ver Personagens</RouterLink>
        </div>
      </section>
      <footer>
        <div class="conteiner-roda">
          <div class="roda-p">
          <p>Fan site – Ben 10 © Cartoon Network</p>
        </div>
        <div class="roda-p">
          <p>Política de Privacidade | Contato</p>
        </div>
      </div>
      </footer> 
</template>

<style scoped>
.series-ben10 {
  text-align: center;
  padding: 2rem;
  position: relative;
  background-color: #111;
}

.container-fundo img {
  width: 100%;
  height: 100%;
  opacity: 0.2;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 0;
  
}

.series-ben10 h2 {
  font-size: 4rem;
  color: #00ff00;
  margin-bottom: 1rem;
  z-index: 1;
  position: relative;
  margin-top: 100px;
}

.serie {
  z-index: 1;
  position: relative;
  max-width: 600px;
  margin: 0 auto;
  background-color: rgba(0, 255, 0, 0.05);
  padding: 1.5rem;
  border: 1px solid #00ff00;
  color: white;

}

.serie p {
  font-size: 1.5rem;
  margin-bottom: 1.5rem;
}

.btn-link {
  display: inline-block;
  margin: 0.5rem;
  padding: 0.7rem 1.5rem;
  background-color: #00ff00;
  color: #000;
  text-decoration: none;
  font-weight: bold;
  font-size: 1.2rem;
  border: none;
}


footer {
  background-color: #000;
  color: #00ff00;
  padding: 1rem 0;
  border-top: 2px solid #00ff00;
  margin-top: 0rem;
  height: 119px;
}

.conteiner-roda {
  max-width: 1000px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  padding: 0 1rem;
  margin-top: 20px;
 
}

.roda-p {
  flex: 1;
  text-align: center;
  padding: 0.5rem;
}

.roda-p p {
  margin: 0;
  font-size: 0.9rem;
}</style>
