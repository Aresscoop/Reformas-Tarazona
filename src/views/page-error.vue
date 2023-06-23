<script>
// import Switcher from "@/components/switcher";
import { HomeIcon } from "vue-feather-icons";

/**
 * Page-error component
 */
export default {
  data() {
    return {};
  },
  components: {
    // Switcher,
    HomeIcon,
  },
};
</script>

<template>
  <div>
    <div class="back-to-home rounded d-none d-sm-block">
      <router-link to="/" class="btn btn-icon btn-soft-primary">
        <home-icon class="icons"></home-icon>
      </router-link>
    </div>

    <!-- ERROR PAGE -->
    <section class="bg-home d-flex align-items-center">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-lg-8 col-md-12 text-center">
            <img src="images/404.svg" class="img-fluid" alt="" />
            <div class="text-uppercase mt-4 display-3">Oh ! no</div>
            <div class="text-capitalize text-dark mb-4 error-page">
              Página no encontrada
            </div>
            <p class="text-muted para-desc mx-auto">
              Parece que algo no funciona, o la página está en mantenimiento,
              vuelve atrás o a la página principal con los botones de abajo.
            </p>
          </div>
          <!--end col-->
        </div>
        <!--end row-->

        <div class="row">
          <div class="col-md-12 text-center">
            <router-link to="/" class="btn btn-outline-primary mt-4"
              >Volver Atrás</router-link
            >
            <router-link to="/" class="btn btn-primary mt-4 ml-2"
              >Página Incio</router-link
            >
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </section>
    <!--end section-->
    <!-- ERROR PAGE -->
    <Switcher />
  </div>
</template>
