<template>
  <div>
    <WhatsappBtn />

    <!-- Header -------------------------------------------------------------------------->
    <header id="home">
      <Navbar/>
        <div class="container p-lg-5 mt-5">
          <div class="hero row p-2">
              <div class="col-lg-5 d-flex flex-column justify-content-center mt-lg-0 mt-4">
                <h3 class="text-secondary">Vellos. Nunca más!</h3>
                <h1>Depilación Láser</h1>
                <p>La depilación láser de diodo es una manera segura,
                    rápida y eficaz de acabar para siempre con las
                    molestias de la depilación tradicional.</p>

                <a href="https://wa.link/ce8hrb" target="_blank" class="btn btn-primary btn-reserve">
                  <fa icon="calendar-check" />
                  RESERVAR TU CITA AQUÍ
                </a>
              </div>

              <div class="col-lg-7 mt-3 mt-lg-0">
                <img src="images/hero.webp" class="img-fluid" alt="hero">
              </div>
          </div>
        </div>
    </header>


    <!-- Service -------------------------------------------------------------------------->
    <section class="bg-light" id="servicios">
      <div class="container py-5">

        <div class="row py-4">
          <div class="col-12 text-center">
            <h2>!Piel Suave Definitiva!</h2>
          </div>
        </div>

        <CardService />
      </div>
    </section>


    <!-- Beneficios -------------------------------------------------------------------------->
    <section>
      <div class="container py-5">
        <div class="row">

          <div class="col-12 text-center">
            <h2 class="text-secondary">Beneficios de la Depilación Láser</h2>
          </div>
        </div>

        <div class="row justify-content-md-center pt-lg-5" >
          <div class="col-12 text-center d-lg-none">
            <img class="img-fluid" src="images/machine.webp" alt="maquina" width="200">
          </div>

          <CardBenefit :benefits="benefits" />

          <div class="col-2 d-none text-center d-lg-flex align-items-center">
            <img class="img-fluid" src="images/machine.webp" alt="maquina">
          </div>

          <CardBenefit :benefits="benefits_two" />
        </div>

      </div>
    </section>


    <!-- Promociones -------------------------------------------------------------------------->
    <section class="bg-light" id="promociones">
      <div class="container py-5">

        <div class="row py-4">
          <div class="col-12 text-center">
            <h2>Promociones</h2>
          </div>
        </div>

        <CardPromos />

      </div>
    </section>


    <!-- Menu -------------------------------------------------------------------------->
    <section class="menu" id="menu">
      <div class="container py-5">
        <div class="row justify-content-md-center py-5">
          <div class="col-12 col-md-4 text-center">
            <h2 class="text-secondary">Menú</h2>
            <p>Descargá nuestro menú con todos los tratamientos que ofrecemos.</p>
            <button class="btn btn-primary px-5 py-2">
                <fa icon="download" /> Descargar
            </button>
          </div>
        </div>
      </div>
    </section>

    <!-- Menu -------------------------------------------------------------------------->
    <section class="consultas" id="contacto">
      <div class="container py-4">
        <div class="row py-3 align-items-center">
            <div class="col-md-4 wow animate__fadeInUp" data-wow-duration="1s">
                <h2 class="m-0 text-white">Consultas?</h2>
                <p>estamos para ayudarte</p>
            </div>

            <div class="col-6 col-md-4 pt-3 p-md-0 text-md-center wow animate__fadeIn" data-wow-duration="1s" data-wow-delay="0.5s">
                <a href="https://wa.link/ce8hrb" target="_blank">
                  <img src="images/icons/icon-whatsapp.svg" alt="icon-what">0981196291
                </a>
            </div>

            <div class="col-6 col-md-4 pt-3 p-md-0 wow animate__fadeIn" data-wow-duration="1s" data-wow-delay="0.5s">
                <a href="https://goo.gl/maps/f3wPMPJbPgz8RN268" target="_blank">
                  <img src="images/icons/icon-maker.svg" alt="icon-maker">Ver ubicación
                </a>
            </div>
        </div>
      </div>
    </section>

    <SecFooter />

  </div>
</template>

<script>
import secFooter from '~/components/sec-footer.vue'
export default {
  components: { secFooter },
  name: 'IndexPage',
  data() {
    return {

      benefits: [
        {src: 'images/icons/icon-laser-1.webp', text: 'Eliminación del vello de manera definitiva' },
        {src: 'images/icons/icon-laser-2.webp', text: 'Adiós a los vellos enterrados' },
        {src: 'images/icons/icon-laser-3.webp', text: 'No maltrata tu piel' },
      ],
      benefits_two: [
        {src: 'images/icons/icon-laser-6.webp', text: 'Ahorro a largo plazo' },
        {src: 'images/icons/icon-laser-5.webp', text: 'Poros cerrados' },
        {src: 'images/icons/icon-laser-4.webp', text: 'Piel más suave' },
      ],

    }
  },
  methods: {

  },
}
</script>

<style lang="scss">
.hero{
  h3{font-weight: 600;}
  .btn-reserve{padding: .5rem}
}
</style>
