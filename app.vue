<script setup>
import BButton from '@compromis/blobby/components/button/BButton.vue'

</script>

<template>
  <div>
    <nav class="app-nav">
      <a href="https://jovespv.org"><jovespv-logo /></a>
      <div class="ms-auto text-lg d-none d-md-inline">IV Congrés de Joves PV</div>
    </nav>
    <div class="content">
      <div class="text-3xl">
        <ser-logo />
        <div class="mt-5 lh-sm">
          19 de febrer 2022
        </div>
        <div class="lh-sm">
          Ontinyent, la Vall d’Albaida
        </div>
      </div>
      <div class="md-d-flex mt-5">
        <b-button href="#" size="lg" variant="primary" has-shadow outline class="me-2 mb-2">Inscriu-te a l'acte</b-button>
        <b-button href="#" size="lg" variant="primary" has-shadow outline class="me-2 mb-2">Esmenes</b-button>
        <b-button href="#" size="lg" variant="primary" has-shadow outline class="me-2 mb-2">Noseque</b-button>
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