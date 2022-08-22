<template>
  <div class="row pb-4 justify-content-md-center">
    <div class="col-12 col-lg-3 mt-3 mt-lg-0 d-flex align-self-stretch"
      v-for="(promo, i) in promotions"
      :key="i">

      <div class="card border-0">
        <img :src="promo.url" class="card-img-top" :alt="promo.title">
        <div class="card-body">
          <h4 class="m-0">{{ promo.title }}</h4>
          <p>{{ promo.description }}</p>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        promotions: []
      }
    },
    created(){
      this.getPromotions();
    },
    methods:{
      getPromotions(){
        this.$axios.$get('/promotions')
          .then(resp => this.promotions = resp.docs)
      }
    }
  }
</script>

<style lang="scss">
  h4{color: #D52084; font-weight:600}
</style>
