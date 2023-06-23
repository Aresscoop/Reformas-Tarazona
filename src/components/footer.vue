<script>
import {
  FacebookIcon,
  InstagramIcon,
  ApertureIcon,
  LinkedinIcon,
  MailIcon,
} from "vue-feather-icons";
export default {
  data() {
    return {};
  },
  components: {
    FacebookIcon,
    InstagramIcon,
    ApertureIcon,
    LinkedinIcon,
    MailIcon,
  },
};
</script>

<template>
  <div>
    <!-- Footer Start -->
    <footer class="footer">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-lg-4 col-12 mb-0 mb-md-4 pb-0 pb-md-2">
            <a href="#" class="logo-footer">
              <img
                src="../../public/images/Logo_horiz_RT_blanco.png"
                width="200"
                height="auto"
                alt=""
              />
            </a>
            <p class="mt-4">
              En Reformas Tarazona realizamos todo tipo de reformas, desde tu
              cocina a tu baño, cambiando azulejos, parquet, muebles, mamparas,
              etc.
            </p>
            <ul class="list-unstyled social-icon social mb-0 mt-4">
              <li class="list-inline-item">
                <a
                  href="https://www.facebook.com/reformastarazona/about?locale=es_ES"
                  target="_blank"
                  class="rounded"
                >
                  <facebook-icon class="fea icon-sm fea-social"></facebook-icon>
                </a>
              </li>
              <li class="list-inline-item ml-1">
                <a
                  href="https://www.instagram.com/reformastarazona/"
                  target="_blank"
                  class="rounded"
                >
                  <instagram-icon
                    class="fea icon-sm fea-social"
                  ></instagram-icon>
                </a>
              </li>
              <li class="list-inline-item ml-1">
                <a
                  href="https://www.pinterest.es/reformastarazona/"
                  target="_blank"
                  class="rounded"
                >
                  <aperture-icon class="fea icon-sm fea-social"></aperture-icon>
                </a>
              </li>
              <li class="list-inline-item ml-1">
                <a
                  href="https://es.linkedin.com/in/reformas-paco-tarazona-67828429"
                  target="_blank"
                  class="rounded"
                >
                  <linkedin-icon class="fea icon-sm fea-social"></linkedin-icon>
                </a>
              </li>
              <li class="fab fa-pinterest"></li>
            </ul>
            <!--end icon-->
          </div>
          <!--end col-->

          <div class="col-lg-2 col-md-3 col-12 mt-4 mt-sm-0 pt-2 pt-sm-0">
            <h5 class="text-light footer-head">Páginas</h5>
            <ul class="list-unstyled footer-list mt-4">
              <li>
                <router-link to="/" class="text-foot"
                  ><i class="mdi mdi-chevron-right mr-1"></i>Inicio</router-link
                >
              </li>
              <li>
                <router-link to="proyectos" class="text-foot"
                  ><i class="mdi mdi-chevron-right mr-1"></i>
                  Proyectos</router-link
                >
              </li>
              <li>
                <router-link to="productos" class="text-foot"
                  ><i class="mdi mdi-chevron-right mr-1"></i>
                  Productos</router-link
                >
              </li>
              <li>
                <router-link to="servicios" class="text-foot"
                  ><i class="mdi mdi-chevron-right mr-1"></i>
                  Servicios</router-link
                >
              </li>
              <li>
                <router-link to="contract" class="text-foot"
                  ><i class="mdi mdi-chevron-right mr-1"></i>
                  Contract</router-link
                >
              </li>
              <li>
                <router-link to="contacto" class="text-foot"
                  ><i class="mdi mdi-chevron-right mr-1"></i>
                  Contacto</router-link
                >
              </li>
            </ul>
          </div>
          <!--end col-->

          <div class="col-lg-3 col-md-4 col-12 mt-4 mt-sm-0 pt-2 pt-sm-0">
            <h5 class="text-light footer-head">Textos Legales</h5>
            <ul class="list-unstyled footer-list mt-4">
              <li>
                <router-link to="/politica-de-cookies" class="text-foot"
                  ><i class="mdi mdi-chevron-right mr-1"></i> Política de
                  Cookies</router-link
                >
              </li>
              <li>
                <router-link to="/politica-de-privacidad" class="text-foot"
                  ><i class="mdi mdi-chevron-right mr-1"></i> Política de
                  Privacidad</router-link
                >
              </li>
              <li>
                <router-link to="/proteccion-de-datos" class="text-foot"
                  ><i class="mdi mdi-chevron-right mr-1"></i> Protección de
                  Datos</router-link
                >
              </li>
            </ul>
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </footer>
    <!--end footer-->
    <footer class="footer footer-bar">
      <div class="container text-center">
        <div class="row justify-content-center">
          <div class="col-sm-6">
            <div class="text-sm-left">
              <p class="mb-0">
                © 2023 - {{ new Date().getFullYear() }} Derechos reservados.
                Reformas Tarazona
              </p>
            </div>
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </footer>
    <!--end footer-->
  </div>
</template>
