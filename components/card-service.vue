<template>
  <div class="row pb-4 justify-content-md-center">
    <div class="col-12 col-lg-3 mt-3 mt-lg-0"
      v-for="(service, i) in services"
      :key="i">

      <div class="card border-0">
          <div class="card-body text-center">
            <img class="py-3" :src="service.src" alt="icon" width="80">
            <p>{{service.text}}</p>
          </div>
      </div>

    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        services: [
          {src: 'images/icons/icon-calidad.svg', text: 'Más de 10 años de experiencia en el mercado' },
          {src: 'images/icons/icon-maquina.svg', text: 'Utilizamos equipos con la mejor y última tecnología' },
          {src: 'images/icons/icon-profesionales.svg', text: 'Realizado por profesionales altamente capacitados' },
        ],
      }
    },
}
</script>
