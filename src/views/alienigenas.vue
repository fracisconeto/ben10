<script setup>
import { ref } from 'vue'

import imgBen10 from '../assets/img/classico/ben10-2.png'

import imgChama from '../assets/img/classico/3.png'
import imgQuatroBracos from '../assets/img/classico/1.png'
import imgXlr8 from '../assets/img/classico/2.png'
import imgMassaCinza from '../assets/img/classico/8.png'
import imgDiamante from '../assets/img/classico/5.png'
import imgCoisa from '../assets/img/classico/6.png'
import imgUltraT from '../assets/img/classico/4.png'
import imgFantasmatico from '../assets/img/classico/9.png'
import imgAquatico from '../assets/img/classico/7.png'
import imgInsectoide from '../assets/img/classico/10.png'

// refs das imagens
const chama = ref(imgChama)
const quatroBracos = ref(imgQuatroBracos)
const xlr8 = ref(imgXlr8)
const massaCinza = ref(imgMassaCinza)
const diamante = ref(imgDiamante)
const coisa = ref(imgCoisa)
const ultraT = ref(imgUltraT)
const fantasmatico = ref(imgFantasmatico)
const aquatico = ref(imgAquatico)
const insectoide = ref(imgInsectoide)

// funções individuais
function destransformarChama() { chama.value = imgBen10 }
function destransformarQuatroBracos() { quatroBracos.value = imgBen10 }
function destransformarXlr8() { xlr8.value = imgBen10 }
function destransformarMassaCinza() { massaCinza.value = imgBen10 }
function destransformarDiamante() { diamante.value = imgBen10 }
function destransformarCoisa() { coisa.value = imgBen10 }
function destransformarUltraT() { ultraT.value = imgBen10 }
function destransformarFantasmatico() { fantasmatico.value = imgBen10 }
function destransformarAquatico() { aquatico.value = imgBen10 }
function destransformarInsectoide() { insectoide.value = imgBen10 }
</script>

<template>
  <div class="ali">
    <div class="container-ali">
      <h2>Conheça os 10 Alienígenas Originais</h2>
    </div>

    <div class="alienigenas">
      <div class="card">
        <div class="container-img">
          <img :src="chama" alt="Chama" />
        </div>
        <div class="nome-ali"><h3>Chama</h3></div>
        <button @click="destransformarChama" class="btn-destransforma">Destransforma</button>
        <div class="descricao-ali">
          <p>Um alienígena de fogo vindo do planeta Pyros. Controla e dispara chamas intensas com o corpo em brasa.</p>
        </div>
      </div>

      <div class="card">
        <div class="container-img">
          <img :src="quatroBracos" alt="Quatro Braços" />
        </div>
        <div class="nome-ali"><h3>Quatro Braços</h3></div>
        <button @click="destransformarQuatroBracos" class="btn-destransforma">Destransforma</button>
        <div class="descricao-ali">
          <p>Gigante musculoso de enorme força física, ideal para batalhas pesadas. Pode pular muito alto e causar tremores com impacto.</p>
        </div>
      </div>

      <div class="card">
        <div class="container-img">
          <img :src="xlr8" alt="XLR8" />
        </div>
        <div class="nome-ali"><h3>XLR8</h3></div>
        <button @click="destransformarXlr8" class="btn-destransforma">Destransforma</button>
        <div class="descricao-ali">
          <p>Extremamente rápido, com corpo aerodinâmico e rodas nos pés. É perfeito para fugas rápidas e ataques velozes.</p>
        </div>
      </div>

      <div class="card">
        <div class="container-img">
          <img :src="massaCinza" alt="Massa Cinzenta" />
        </div>
        <div class="nome-ali"><h3>Massa Cinzenta</h3></div>
        <button @click="destransformarMassaCinza" class="btn-destransforma">Destransforma</button>
        <div class="descricao-ali">
          <p>Pequeno e superinteligente. Usa lógica, ciência e estratégia para resolver problemas e hackear qualquer coisa.</p>
        </div>
      </div>

      <div class="card">
        <div class="container-img">
          <img :src="diamante" alt="Diamante" />
        </div>
        <div class="nome-ali"><h3>Diamante</h3></div>
        <button @click="destransformarDiamante" class="btn-destransforma">Destransforma</button>
        <div class="descricao-ali">
          <p>Corpo de cristal superduro. Pode disparar estilhaços, criar armas com os braços e refletir ataques de energia.</p>
        </div>
      </div>

      <div class="card">
        <div class="container-img">
          <img :src="coisa" alt="Coisa" />
        </div>
        <div class="nome-ali"><h3>Coisa</h3></div>
        <button @click="destransformarCoisa" class="btn-destransforma">Destransforma</button>
        <div class="descricao-ali">
          <p>Criatura feroz com sentidos aguçados, mesmo sem olhos. Excelente rastreador e ótimo em combates corpo a corpo.</p>
        </div>
      </div>

      <div class="card">
        <div class="container-img">
          <img :src="ultraT" alt="Ultra T" />
        </div>
        <div class="nome-ali"><h3>Ultra T</h3></div>
        <button @click="destransformarUltraT" class="btn-destransforma">Destransforma</button>
        <div class="descricao-ali">
          <p>Alienígena biomecânico que pode se fundir com tecnologia para melhorá-la e controlá-la. Corpo líquido e metálico.</p>
        </div>
      </div>

      <div class="card">
        <div class="container-img">
          <img :src="fantasmatico" alt="Fantasmático" />
        </div>
        <div class="nome-ali"><h3>Fantasmático</h3></div>
        <button @click="destransformarFantasmatico" class="btn-destransforma">Destransforma</button>
        <div class="descricao-ali">
          <p>Alien fantasmagórico com poder de ficar invisível, atravessar paredes e possuir corpos. Um dos mais sombrios.</p>
        </div>
      </div>

      <div class="card">
        <div class="container-img">
          <img :src="aquatico" alt="Aquático" />
        </div>
        <div class="nome-ali"><h3>Aquático</h3></div>
        <button @click="destransformarAquatico" class="btn-destransforma">Destransforma</button>
        <div class="descricao-ali">
          <p>Veloz e poderoso na água. Possui mandíbulas fortes e nadadeiras retráteis. Excelente para missões subaquáticas.</p>
        </div>
      </div>

      <div class="card">
        <div class="container-img">
          <img :src="insectoide" alt="Insectóide" />
        </div>
        <div class="nome-ali"><h3>Insectóide</h3></div>
        <button @click="destransformarInsectoide" class="btn-destransforma">Destransforma</button>
        <div class="descricao-ali">
          <p>Inseto voador com múltiplos olhos. Dispara gosma pegajosa e é muito ágil no ar. Incomum, mas versátil.</p>
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

<style scoped>
.ali {
  background-color: #111;
}
.container-ali {
  text-align: center;
  padding: 2rem 1rem;
  margin: auto;
}
.container-ali h2 {
  font-size: 2rem;
  color: #00ff00;
}
.alienigenas {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1.5rem;
  padding: 2rem;
  max-width: 1000px;
  margin: 0 auto;
  color: white;
  background-color: #111;
}
.card {
  background-color: #000;
  padding: 1rem;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
}
.container-img img {
  width: 100%;
  height: 200px;
  object-fit: contain;
  background-color: #000;
}
.nome-ali h3 {
  font-size: 1.2rem;
  color: #00ff00;
  margin: 0.5rem 0;
  text-align: center;
}
.descricao-ali {
  height: 100px;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0.5rem;
  background-color: #000;
  margin-top: 0.5rem;
}
.descricao-ali p {
  font-size: 1rem;
  text-align: center;
  line-height: 1.4;
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
.btn-destransforma {
  background-color: #00ff00;
  color: #000;
  font-weight: bold;
  padding: 0.3rem 0.8rem;
  border: none;
  cursor: pointer;
  margin-top: 0.5rem;
  display: block;
  border-radius: 5px;
}
@media (max-width: 768px) {
  .alienigenas {
    grid-template-columns: 1fr;
    padding: 1rem;
  }

  .container-img img {
    height: auto;
    max-height: 250px;
  }

  .descricao-ali {
    height: auto;
  }

  footer {
    height: auto;
    text-align: center;
  }

  .conteiner-roda {
    flex-direction: column;
    align-items: center;
    gap: 0.5rem;
  }

  .roda-p {
    flex: none;
    width: 100%;
  }
}
</style>
