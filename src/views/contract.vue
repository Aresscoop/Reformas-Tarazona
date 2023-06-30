<script>
import {
  ArrowUpIcon,
  MailIcon,
  UserIcon,
  MessageCircleIcon,
} from "vue-feather-icons";

import Navbar from "@/components/navbar";
// import Switcher from "@/components/switcher";
import Footer from "@/components/footer";

/**
 * Page-work-detail component
 */
export default {
  data() {
    return {};
  },
  components: {
    Navbar,
    // Switcher,
    Footer,
    ArrowUpIcon,
    MailIcon,
    UserIcon,
    MessageCircleIcon,
  },
};
</script>

<template>
  <div>
    <Navbar />

    <!-- Hero Start -->
    <section class="bg-half bg-light d-table w-100">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-lg-12 text-center">
            <div class="page-next-level">
              <h1 class="title">Contract</h1>
              <div class="page-next">
                <nav aria-label="breadcrumb" class="d-inline-block">
                  <ul class="breadcrumb bg-white rounded shadow mb-0">
                    <li class="breadcrumb-item">
                      <router-link to="/">Inicio</router-link>
                    </li>
                    <li class="breadcrumb-item active" aria-current="page">
                      Contract
                    </li>
                  </ul>
                </nav>
              </div>
            </div>
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </section>
    <!--end section-->
    <!-- Hero End -->

    <!-- Shape Start -->
    <div class="position-relative">
      <div class="shape overflow-hidden text-white">
        <svg
          viewBox="0 0 2880 48"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M0 48H1437.5H2880V0H2160C1442.5 52 720 0 720 0H0V48Z"
            fill="currentColor"
          ></path>
        </svg>
      </div>
    </div>
    <!--Shape End-->

    <!-- Start Work Detail -->
    <section class="section">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-12 text-center">
            <img
              src="images/work/single.jpg"
              class="img-fluid rounded"
              alt=""
            />
          </div>

          <div class="col-md-10 mt-4 pt-2 text-justify">
            <h2>¿Quieres un diseño único, creado para tí a tu medida?</h2>
            <p>
              El Contract es la solución, crea espacios personalizados y
              adaptados a tu estilo y al espacio, con muebles a medida y una
              decoración en consonancia con el espacio. El Contract busca que
              cada cliente disfrute de una estancia armónica, con un diseño
              exclusivo, al cual se llega tras un estudio del cliente, sus
              necesidades y sus expectativas, creando así proyectos a medida.
            </p>
            <p>
              Este tipo de reforma se diferencia del resto por el tipo de
              mobiliario usado, tanto en sus materiales como en su resistencia,
              diseñados para un uso extremo e intensivo como es el de los
              muebles de la hostelería. Estos muebles cuentan con una gran
              personalización y exigencia. Algunas cualidades del contract son:
              Facilidad de adaptación del estilo y la decoración, Creación de
              atmósferas más acogedoras, Aporte de atractivo visual a los
              espacios, Gran nivel de resistencia y durabilidad, Oferta amplia
              (modelos, colores…) y Perfecta conexión entre decoración,
              interiorismo y comodidad.
            </p>
            <div class="bg-light rounded p-4">
              <p class="text-muted font-italic mb-0">
                En Reformas Trazona sabemos, que en un diseño cada parte del
                mismo cuenta tanto cómo la suma de todas sus partes.
              </p>
            </div>

            <div class="row">
              <div class="col-md-6 mt-4 pt-2">
                <img src="images/work/2.jpg" class="img-fluid rounded" alt="" />
              </div>

              <div class="col-md-6 mt-4 pt-2">
                <img src="images/work/3.jpg" class="img-fluid rounded" alt="" />
              </div>
            </div>

            <div class="row align-items-center">
              <div class="col-lg-6 mt-4 pt-2">
                <div class="card work-details rounded bg-light border-0">
                  <div class="card-body">
                    <h5 class="card-title border-bottom pb-3 mb-3">
                      Info. del Proyecto:
                    </h5>
                    <dl class="row mb-0">
                      <dt class="col-md-4 col-5">Client :</dt>
                      <dd class="col-md-8 col-7 text-muted">Calvin Carlo</dd>

                      <dt class="col-md-4 col-5">Category :</dt>
                      <dd class="col-md-8 col-7 text-muted">Web Design</dd>

                      <dt class="col-md-4 col-5">Date :</dt>
                      <dd class="col-md-8 col-7 text-muted">23rd Sep, 2019</dd>

                      <dt class="col-md-4 col-5">Website :</dt>
                      <dd class="col-md-8 col-7 text-muted">
                        www.yourdomain.com
                      </dd>

                      <dt class="col-md-4 col-5">Location :</dt>
                      <dd class="col-md-8 col-7 text-muted">
                        3/2/64 Mongus Street, UK
                      </dd>
                    </dl>
                  </div>
                </div>
              </div>

              <div class="col-lg-6 mt-4 pt-2">
                <img src="images/work/6.jpg" class="img-fluid rounded" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Project Start -->
    <section class="section bg-light">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-12 text-center">
            <div class="section-title mb-4 pb-2">
              <h4 class="title mb-4">Proyectos de Contract</h4>
              <p class="text-muted para-desc mx-auto mb-0">
                Contamos con un amplia experiencia en el sector de las reformas
                Contract, aquí puedes ver algunos de nuestros trabajos ya
                realizados.
              </p>
            </div>
          </div>
          <!--end col-->
        </div>
        <!--end row-->

        <div class="row">
          <div class="col-md-6 col-12 mt-4 pt-2">
            <div
              class="card work-container work-modern position-relative overflow-hidden shadow rounded border-0"
            >
              <div class="card-body p-0">
                <img
                  src="images/work/1.jpg"
                  class="img-fluid rounded"
                  alt="work-image"
                />
                <div class="overlay-work bg-dark"></div>
                <div class="content">
                  <router-link
                    to="/page-work-detail"
                    class="title text-white d-block font-weight-bold"
                    >Shifting Perspective</router-link
                  >
                  <small class="text-light">Studio</small>
                </div>
                <div class="client">
                  <small class="text-light user d-block"
                    ><i class="mdi mdi-account"></i> Calvin Carlo</small
                  >
                  <small class="text-light date"
                    ><i class="mdi mdi-calendar-check"></i> 13th August,
                    2019</small
                  >
                </div>
              </div>
            </div>
          </div>
          <!--end col-->

          <div class="col-md-6 col-12 mt-4 pt-2">
            <div
              class="card work-container work-modern position-relative overflow-hidden shadow rounded border-0"
            >
              <div class="card-body p-0">
                <img
                  src="images/work/2.jpg"
                  class="img-fluid rounded"
                  alt="work-image"
                />
                <div class="overlay-work bg-dark"></div>
                <div class="content">
                  <router-link
                    to="/page-work-detail"
                    class="title text-white d-block font-weight-bold"
                    >Colors Magazine</router-link
                  >
                  <small class="text-light">Web Design</small>
                </div>
                <div class="client">
                  <small class="text-light user d-block"
                    ><i class="mdi mdi-account"></i> Calvin Carlo</small
                  >
                  <small class="text-light date"
                    ><i class="mdi mdi-calendar-check"></i> 13th August,
                    2019</small
                  >
                </div>
              </div>
            </div>
          </div>
          <!--end col-->

          <div class="col-md-6 col-12 mt-4 pt-2">
            <div
              class="card work-container work-modern position-relative overflow-hidden shadow rounded border-0"
            >
              <div class="card-body p-0">
                <img
                  src="images/work/3.jpg"
                  class="img-fluid rounded"
                  alt="work-image"
                />
                <div class="overlay-work bg-dark"></div>
                <div class="content">
                  <router-link
                    to="/page-work-detail"
                    class="title text-white d-block font-weight-bold"
                    >Spa Cosmetics</router-link
                  >
                  <small class="text-light">Developing</small>
                </div>
                <div class="client">
                  <small class="text-light user d-block"
                    ><i class="mdi mdi-account"></i> Calvin Carlo</small
                  >
                  <small class="text-light date"
                    ><i class="mdi mdi-calendar-check"></i> 13th August,
                    2019</small
                  >
                </div>
              </div>
            </div>
          </div>
          <!--end col-->

          <div class="col-md-6 col-12 mt-4 pt-2">
            <div
              class="card work-container work-modern position-relative overflow-hidden shadow rounded border-0"
            >
              <div class="card-body p-0">
                <img
                  src="images/work/4.jpg"
                  class="img-fluid rounded"
                  alt="work-image"
                />
                <div class="overlay-work bg-dark"></div>
                <div class="content">
                  <router-link
                    to="/page-work-detail"
                    class="title text-white d-block font-weight-bold"
                    >Riser Coffee</router-link
                  >
                  <small class="text-light">Branding</small>
                </div>
                <div class="client">
                  <small class="text-light user d-block"
                    ><i class="mdi mdi-account"></i> Calvin Carlo</small
                  >
                  <small class="text-light date"
                    ><i class="mdi mdi-calendar-check"></i> 13th August,
                    2019</small
                  >
                </div>
              </div>
            </div>
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </section>
    <!--end section-->
    <!-- Project End -->
    <!-- End Work Detail -->
    <!--end section-->
    <Footer />
    <!-- Footer End -->
    <Switcher />
    <!-- Back to top -->
    <a
      href="javascript: void(0);"
      class="btn btn-icon btn-primary back-to-top"
      id="back-to-top"
      v-scroll-to="'#topnav'"
    >
      <arrow-up-icon class="icons"></arrow-up-icon>
    </a>
    <!-- Back to top -->
  </div>
</template>
