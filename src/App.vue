<script setup>
import BButton from '@compromis/blobby/components/button/BButton.vue'
import JovespvLogo from './components/JovespvLogo.vue'
import AvantLogo from './components/AvantLogo.vue'
</script>

<template>
  <div>
    <nav class="app-nav">
      <a href="https://jovespv.org" title="Joves PV"><jovespv-logo /></a>
      <div class="ms-auto text-lg">V Congrés de Joves PV</div>
    </nav>
    <div class="content">
      <div class="text-3xl">
        <avant-logo class="avant" />
        <span class="visually-hidden">Avant</span>
        <div class="mt-5 lh-sm opacity-50 info">
          10 de febrer de 2024
        </div>
        <div class="lh-sm opacity-50 info">
          Vilanova d'Alcolea
        </div>
      </div>
      <div class="md-d-flex mt-5">
        <a href="https://forms.gle/iwxYNbNdV9wp9qaD7" target="_blank" class="avant-button avant-blue me-3 mb-2">
          Inscripció al Congrés
        </a>
        <a href="https://esmenes.compromis.net/jovespv" target="_blank" class="avant-button avant-red mb-2">
          Esmenes i documents
        </a>
      </div>
      <div class="text text-xl mt-4">
        <p>La corrupció i el feixisme han tornat a apoderar-se de les institucions valencianes. Això ens obliga a fer front a molts reptes als i les joves del País Valencià.</p>
        <p>Ara ens trobem davant del moment de celebrar un nou Congrés; obert a totes les persones joves, siguen militants del nostre partit o no. I això t’inclou també a tu. Com a organització, encetem el nostre període de reflexió més significatiu: una oportunitat per replantejar-nos, per reforçar-nos i decidir què volem ser en aquests temps tan desafiants que ens esperen.</p>
        <p>És una oportunitat per compartir idees, debatre sobre les qüestions més rellevants i prendre decisions que marcaran el nostre camí. Siga quina siga la teua relació amb Joves PV, la teua presència i participació són importants per construir un futur conjunt que reflectisca les nostres aspiracions i valors compartits, i que done esperança a les futures generacions de valencianes i valencians.</p>
        <p>Vos convidem a participar en aquest esdeveniment que serà clau per definir els rumbs de Joves PV i del País Valencià d’ara en avant. Ens veiem al Congrés el 10 de febrer a Vilanova d’Alcolea! "(en cursiva text que igual no cal si ja apareix en primera plana del web la data i el lloc)</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@import '@compromis/blobby/scss/blobby.scss';
@import './assets/scss/variables';

body, html {
  background: #231f20;
  color: #fff;
  font-family: "itc-avant-garde-gothic-pro", sans-serif;
  font-weight: 300;
}

.app-nav {
  position: fixed;
  display: flex;
  align-items: center;
  padding: .5rem 1rem;
  top: 0;
  left: 0;
  right: 0;

  svg {
    height: 2rem;
    width: fit-content;
  }
}

.content {
  padding: 1rem;
  max-width: 800px;
  margin: 15vh auto;

  svg {
    width: 100%;
    height: auto;
  }
}

.opacity-50 {
  opacity: .5;
}

.avant-blue {
  --color: #{$blue};
}

.avant-red {
  --color: #{$green};
}

.avant-button {
  display: inline-flex;
  border: 2px var(--color) solid;
  color: var(--color);
  padding: .5rem .75rem;
  font-size: 1.25rem;
  font-weight: 700;

  &:hover {
    background: var(--color);
    color: $white;
    text-decoration: none;
  }
}

@media (max-width: 1050px) {
  .app-nav {
    position: static;
  }
}

@media (max-width: 750px) {
  .app-nav {
    .text-lg {
      font-size: 1rem;
    }
  }

  .info {
    font-size: 1.5rem;
  }
}
</style>
