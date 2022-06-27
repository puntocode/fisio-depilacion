<template>
  <div class="navbar-area bg-ligth d-block">
    <nav class="navbar navbar-expand-lg navbar-light bg-white w-100 fixed-top" id="navbar">
        <div class="container">
            <a href="#home" class="navbar-brand text-uppercase"><img src="/images/logo-depi.svg" width="180"></a>

            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
              <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarNavDropdown">
              <ul class="navbar-nav w-100 justify-content-end">
                  <li class="nav-item">
                      <a class="nav-link active" href="#home">Inicio</a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link" href="#servicios">Servicios</a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link" href="#promociones">Promociones</a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link" href="#menu">Menú</a>
                  </li>
                  <li class="nav-item">
                      <a class="nav-link" href="#contacto">Contacto</a>
                  </li>
              </ul>
            </div>

          </div>
      </nav>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
  .navbar-area{min-height: 40px;
    .navbar-nav{font-weight: 600;
      .nav-item{padding-left: 1rem;}
    }
  }
</style>

