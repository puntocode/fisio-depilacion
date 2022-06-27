<template>
  <div class="row pb-4 justify-content-md-center">
    <div class="col-12 col-lg-3 mt-3 mt-lg-0 d-flex align-self-stretch"
      v-for="(promo, i) in promociones"
      :key="i">

      <div class="card border-0">
        <img :src="promo.src" class="card-img-top" alt="...">
        <div class="card-body">
          <h4 class="m-0">{{ promo.title }}</h4>
          <p>{{ promo.text }}</p>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        promociones: [
          {src: 'https://static1.abc.es/media/summum/2019/10/04/depilacion-keRB--1200x630@abc.jpg', title: '2x1', text: 'Espalda' },
          {src: 'https://static1.abc.es/media/summum/2019/10/04/depilacion-keRB--1200x630@abc.jpg', title: '20% OFF', text: 'Para hombres' },
          {src: 'https://static1.abc.es/media/summum/2019/10/04/depilacion-keRB--1200x630@abc.jpg', title: 'Mes de Papá', text: 'Comprando el paquete de abdomen, te llevas axilas gratis' },
        ]
      }
    },
  }
</script>

<style lang="scss">
  h4{color: #D52084; font-weight:600}
</style>
