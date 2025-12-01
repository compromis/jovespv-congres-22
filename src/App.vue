<script setup>
import BButton from '@compromis/blobby/components/button/BButton.vue'
import JovespvLogo from './components/JovespvLogo.vue'
import AvantLogo from './components/AvantLogo.vue'
</script>

<template>
  <div>
    <nav class="app-nav">
      <a href="https://jovespv.org" title="Joves PV"><jovespv-logo /></a>
      <div class="ms-auto text-lg">VI Congrés de Joves PV</div>
    </nav>
    <div class="content">
      <div class="text-3xl">
        <h1>VI Congrés de Joves PV</h1>
        <div class="mt-5 lh-sm opacity-50 info">
          21 de febrer de 2026
        </div>
        <div class="lh-sm opacity-50 info">
          Àgora, Alcoi
        </div>
      </div>
      <div class="md-d-flex mt-5">
        <!--<a href="https://forms.gle/iwxYNbNdV9wp9qaD7" target="_blank" class="avant-button avant-blue me-3 mb-2">
          Inscripció al Congrés
        </a>-->
        <a href="https://esmenes.compromis.net/jovespv-2026" target="_blank" class="avant-button avant-orange mb-2">
          Esmenes i documents
        </a>
      </div>
      <div class="text text-xl mt-4">
        <p>Després dels canvis que ha viscut el País Valencià els últims dos anys, ara ens trobem davant del moment de celebrar un nou Congrés; obert a totes les persones joves, siguen militants del nostre partit o no. I això t’inclou també a tu. </p>

        <p>Com a organització, encetem el nostre període de reflexió més significatiu: una oportunitat per replantejar-nos, per reforçar-nos i decidir què volem ser en aquests temps tan desafiants que ens esperen.</p>

        <p>És una oportunitat per compartir idees, debatre sobre les qüestions més rellevants i prendre decisions que marcaran el nostre camí. Siga quina siga la teua relació amb Joves PV, la teua presència i participació són importants per construir un futur conjunt que reflectisca les nostres aspiracions i valors compartits, i que done esperança a les futures generacions de valencianes i valencians.</p>

        <p>Vos convidem a participar en aquest esdeveniment que serà clau per definir els rumbs de Joves PV i del País Valencià. Ens veiem al VI Congrés de Joves PV el 21 de febrer a Alcoi!      </p>
    </div>
    </div>
  </div>
</template>

<style lang="scss">
@import '@compromis/blobby/scss/blobby.scss';
@import './assets/scss/variables';

body, html {
  background: $white;
  color: $black;
  font-family: "itc-avant-garde-gothic-pro", sans-serif;
  font-weight: 300;
}

.app-nav {
  position: fixed;
  display: flex;
  align-items: center;
  padding: 1rem;
  top: 0;
  left: 0;
  right: 0;
  z-index: 100;

  svg {
    height: 2rem;
    width: auto;
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

.avant-orange {
  --color: #{$orange};
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
    background-color: $black;
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
