
<template>
  <footer class="footer">
    <div class="container py-5">

        <div class="row border-bottom">
            <div class="col-lg-3 text-center text-lg-start wow animate__fadeInLeftBig" data-wow-duration="1s">
                <img src="images/logo-white.svg" alt="logo de la empresa" class="logo">
                <div class="mt-lg-4 mb-4">
                    <a href="https://www.facebook.com/fisiostetik">
                      <img class="icon-invert" src="images/icons/icon-facebook.svg" alt="icono de facebook" width="30">
                    </a>
                    <a href="https://www.instagram.com/fisiostetik">
                      <img class="icon-invert"  src="images/icons/icon-instagram.svg" alt="icono de instagram" width="30">
                    </a>
                </div>
            </div>

            <div class="col-lg-3 mb-4 wow animate__fadeInLeftBig" data-wow-duration="1s" data-wow-delay="0.3s">
                <h4 class="text-white">Mapa del Sitio</h4>
                <ul class="accesos">
                    <li><a href="/#home">Inicio</a></li>
                    <li><a href="/#servicios">Servicios</a></li>
                    <li><a href="/#portfolio">Portfolio</a></li>
                    <li><a href="">Blog</a></li>
                </ul>
            </div>

            <div class="col-lg-3 mb-4 wow animate__fadeInLeftBig" data-wow-duration="1s" data-wow-delay="0.5s">
                <h4 class="text-white">Formas de Pago</h4>
                <div class="pe-lg-4">
                    <img height="30" class="me-1 icon-invert" src="images/icons/icon-qr.svg" alt="Pago QR">
                    <img height="30" class="m-1" src="images/icons/icon-mastercard.svg" alt="pago con mastercard">
                    <img height="30" class="m-1" src="images/icons/icon-visa.svg" alt="pago con visa">
                    <img height="30" class="m-1" src="images/icons/icon-amex.svg" alt="pago con american">
                    <img height="30" class="m-1" src="images/icons/icon-efectivo.svg" alt="pago con efectivo">
                    <img height="30" class="m-1" src="images/icons/icon-billetera-personal.svg" alt="billetera personal">
                    <img height="30" class="m-1" src="images/icons/icon-tigo-money.svg" alt="Tigo Money">
                </div>
            </div>

            <div class="col-lg-3 my-4 mt-lg-0 wow animate__fadeInLeftBig" data-wow-duration="1s" data-wow-delay="0.7s">
                <h4 class="text-white">Contáctenos</h4>
                <ul class="accesos">
                    <li v-for="contacto in contactos" :key="contacto.icon">
                        <a :href="contacto.link" target="_blank">
                          <img class="icon-invert pe-1" :src="contacto.img" :alt="`icono de ${contacto.icon}`" width="25">
                          {{ contacto.text }}
                        </a>
                    </li>
                </ul>
            </div>
        </div>

        <div class="row pt-3">
          <div class="col-md-6 text-center text-md-start">
            <p>Desarrollado por:
              <a class="text-punto" href="http://puntocode.com.py" target="_blank">PUNTOCODE</a>
            </p>
          </div>
          <div class="col-md-6 text-md-end text-center">
            <p>&copy; {{year}} Todos los derechos reservados</p>
          </div>
        </div>
    </div>
</footer>
</template>

<script>
export default {
  data() {
    return {
      contactos: [
        {link: 'https://wa.link/ce8hrb', img: 'images/icons/icon-contacto-whatsapp.svg', icon: 'whatsapp', text: '0981196291'},
        {link: 'https://wa.link/b13x2v', img: 'images/icons/icon-contacto-gmail.svg', icon: 'email', text: 'fisiostetik.py@gmail.com'},
        {link: 'https://wa.link/b13x2v', img: 'images/icons/icon-contacto-web.svg', icon: 'web', text: 'www.fisiostetik.com.py'},
        {link: 'https://wa.link/b13x2v', img: 'images/icons/icon-contacto-map.svg', icon: 'mapa', text: 'Campos Cervera 5175'}
      ],
      year: new Date().getFullYear()
    }
  },
}
</script>
