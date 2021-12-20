<script setup>
import BButton from '@compromis/blobby/components/button/BButton.vue'
import thumbnail from '../assets/og.jpeg'
const title = "IV Congrés de Joves PV - Compromís"
const description = ""
const url = "https://congres.jovespv.org"
const image = url + thumbnail
</script>

<template>
  <div>
    <Head lang="ca">
      <Title>{{ title }}</Title>
      <Meta name="description" :content="description" />
      <Meta name="keywords" content="joves pv, compromis, congrés, ser" />
      <Meta name="robots" content="index, follow" />

      <Meta name="og:locale" content="ca" />
      <Meta name="og:type" content="website" />
      <Meta name="og:description" :content="description" />
      <Meta name="og:image" :content="image" />
      <Meta name="og:url" :content="url" />
      <Meta name="twitter:site" content="@jovespv" />
      <Meta name="twitter:card" content="summary_large_image" />
      <Meta name="twitter:title" :content="title" />
      <Meta name="twitter:description" :content="description" />
      <Meta name="twitter:image" :content="image" />
      <Meta name="twitter:url" :content="url" />
    </Head>
    <nav class="app-nav">
      <a href="https://jovespv.org" title="Joves PV"><jovespv-logo /></a>
      <div class="ms-auto text-lg d-none d-md-inline">IV Congrés de Joves PV</div>
    </nav>
    <div class="content">
      <div class="text-3xl">
        <ser-logo />
        <span class="visually-hidden">Ser</span>
        <div class="mt-5 lh-sm">
          19 de febrer 2022
        </div>
        <div class="lh-sm">
          Ontinyent, la Vall d’Albaida
        </div>
      </div>
      <div class="md-d-flex mt-5">
        <b-button href="https://esmenes.compromis.net/jovespv" target="_blank" size="lg" variant="primary" has-shadow outline class="me-2 mb-2">
          Esmenes
        </b-button>
        <b-button href="https://forms.gle/5K95cNmiwJ6NQwbP9" target="_blank" size="lg" variant="primary" has-shadow outline class="me-2 mb-2">
          Inscripció al Congrés
        </b-button>
        <b-button href="https://forms.gle/wRmjawae2PuvgyVJ6" target="_blank" size="lg" variant="primary" has-shadow outline class="me-2 mb-2">
          Inscripció acte homenatge
        </b-button>
      </div>
      <div class="text text-xl mt-4">
        Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. 
        Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem.
        Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?
      </div>
    </div>
    <jovespv-star class="joves-pv-star" />
  </div>
</template>

<style lang="scss">
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