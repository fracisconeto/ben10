<script setup>
import benImg from '../assets/img/classico/ben10.png'
import gwenImg from '../assets/img/classico/gwen.png'
import maxImg from '../assets/img/classico/max.png'
import vilaoImg from '../assets/img/classico/vilão.png'
</script>

<template>
  <div class="black">
    <div class="container-ali">
      <h2>Personagens Principais</h2>
    </div>

    <div class="personagens">

      <div class="card">
        <div class="container-img">
          <img v-if="benImg" :src="benImg" alt="Ben Tennyson" />
        </div>
        <div class="nome-ali">
          <h3>Ben Tennyson</h3>
        </div>
        <div class="descricao-ali">
          <p>
            Um garoto de 10 anos que encontra o Omnitrix. Com coragem e atitude, se transforma em diversos heróis alienígenas.
          </p>
        </div>
      </div>

      <div class="card">
        <div class="container-img">
          <img v-if="gwenImg" :src="gwenImg" alt="Gwen Tennyson" />
        </div>
        <div class="nome-ali">
          <h3>Gwen Tennyson</h3>
        </div>
        <div class="descricao-ali">
          <p>
            Prima de Ben, muito inteligente e habilidosa com magia e tecnologia. Ajuda nas estratégias do grupo.
          </p>
        </div>
      </div>

      <div class="card">
        <div class="container-img">
          <img v-if="maxImg" :src="maxImg" alt="Vô Max" />
        </div>
        <div class="nome-ali">
          <h3>Vô Max</h3>
        </div>
        <div class="descricao-ali">
          <p>
            Avô de Ben e Gwen. Ex-encanador que conhece vários segredos sobre aliens. É o guia e protetor da dupla.
          </p>
        </div>
      </div>

      <div class="card">
        <div class="container-img">
          <img v-if="vilaoImg" :src="vilaoImg" alt="Vilgax" />
        </div>
        <div class="nome-ali">
          <h3>Vilgax</h3>
        </div>
        <div class="descricao-ali">
          <p>
            Um dos maiores inimigos de Ben. Vilgax é um conquistador alienígena que quer o poder do Omnitrix a todo custo.
          </p>
        </div>
      </div>

    </div>
  </div>

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


<style scoped>@import url('https://fonts.googleapis.com/css2?family=Michroma&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
 
  }
  
  body {
    font-family: "Michroma", sans-serif;

    background-color: #111;
    color: #fff;
  }
  
.black{
    background-color: #111;
    
}
  
  /* Título */
  .container-ali {
    text-align: center;
    padding: 20px 0;
    
  }
  
  .container-ali h2 {
    font-size: 28px;
    color: #00ff00;
  }
  
  /* Cards */
  .personagens {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    padding: 30px;
  }
  
  .card {
    background-color: #000;
    width: 300px;
    padding: 15px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  .container-img img {
    width: 200px;
    height: 200px;
    object-fit: contain;
    margin-bottom: 10px;
  }
  
  .nome-ali h3 {
    font-size: 20px;
    color: #00ff00;
    margin-bottom: 8px;
    text-align: center;
  }
  
  .descricao-ali p {
    font-size: 14px;
    line-height: 1.4;
    text-align: center;
    min-height: 60px;
    color:white
  }
  footer {
  background-color: #000;
  color: #00ff00;
  padding: 1rem 0;
  border-top: 2px solid #00ff00;
  margin-top: 0rem;
  height: 135px;
}

.conteiner-roda {
  max-width: 1000px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  padding: 0 1rem;
  margin-top: 20px;
  color: #00ff00
}

.roda-p {
  flex: 1;
  text-align: center;
  padding: 0.5rem;
}

.roda-p p {
  margin: 0;
  font-size: 0.9rem;
}
  </style>