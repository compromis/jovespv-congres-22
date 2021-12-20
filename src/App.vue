<script setup>
import BButton from '@compromis/blobby/components/button/BButton.vue'
import JovespvLogo from './components/JovespvLogo.vue'
import JovespvStar from './components/JovespvStar.vue'
import SerLogo from './components/SerLogo.vue'
</script>

<template>
  <div>
    <nav class="app-nav">
      <a href="https://jovespv.org" title="Joves PV"><jovespv-logo /></a>
      <div class="ms-auto text-lg d-none d-md-inline">IV Congrés de Joves PV</div>
    </nav>
    <div class="content">
      <div class="text-3xl">
        <ser-logo />
        <span class="visually-hidden">Ser</span>
        <div class="mt-5 lh-sm">
          19 de febrer de 2022
        </div>
        <div class="lh-sm">
          Ontinyent, la Vall d’Albaida
        </div>
      </div>
      <div class="md-d-flex mt-5">
        <b-button href="https://forms.gle/ku6hSqgBPfRf3AiG6" target="_blank" size="lg" variant="primary" has-shadow outline class="me-3 mb-2">
          Inscripció al Congrés
        </b-button>
        <b-button href="https://esmenes.compromis.net/jovespv" target="_blank" size="lg" variant="primary" has-shadow outline class="mb-2">
          Esmenes
        </b-button>
      </div>
      <div class="text text-xl mt-4">
        <p>Viure aquests 2 anys no ha estat fàcil. Totes hem patit dificultats per ser allò que érem i ens hem hagut de reinventar a nosaltres mateixa. Així, la pandèmia ens ha obligat a canviar la nostra manera de fer política. Malgrat tot, hem aconseguit fer de <strong>Joves PV</strong> l’espai que ha sostingut la nostra militància, conviccions, lligams i, en molts casos, amistats.</p>
        <p>Ara, ha aplegat el moment de celebrar un nou <strong>Congrés</strong>. Un Congrés al que pot assistir qualsevol jove, siga militant o no. Tu també.</p>
        <p>Com a organització obrim el nostre major període de reflexió: una nova oportunitat per a repensar-nos, per a fer-nos més fortes i decidir tot allò que volem <strong>ser</strong> en els temps tan desafiants que vénen.</p>
      </div>
    </div>
    <jovespv-star class="joves-pv-star" />
  </div>
</template>

<style lang="scss">
@import '@compromis/blobby/scss/blobby.scss';

body, html {
  background: transparent;
}

.app-nav {
  display: flex;
  align-items: center;
  padding: .5rem 1rem;

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
    max-width: 350px;
    height: auto;
  }
}

.joves-pv-star {
  position: fixed;
  width: 35vw;
  bottom: 0;
  right: 0;
  z-index: -1;
}
</style>
