<script>
import {
  ArrowUpIcon,
  MailIcon,
  UserIcon,
  MessageCircleIcon,
} from "vue-feather-icons";

import Navbar from "@/components/ca/navbar";
// import Switcher from "@/components/switcher";
import Footer from "@/components/ca/footer";

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
                      <router-link to="/">Inici</router-link>
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
            <h2>Vols un disseny únic, creat per a *tí a la teua mesura?</h2>
            <p>
              El Contract és la solució, crea espais personalitzats i adaptats
              al teu estil i a l'espai, amb mobles a mesura i una decoració
              d'acord amb l'espai. El Contract busca que cada client gaudisca
              d'una estada harmònica, amb un disseny exclusiu, al qual s'arriba
              després d'un estudi del client, les seues necessitats i les seues
              expectatives, creant així projectes a mesura.
            </p>
            <p>
              Aquest tipus de reforma es diferencia de la resta pel tipus de
              mobiliari usat, tant en els seus materials com en la seua
              resistència, dissenyats per a un ús extrem i intensiu com és el
              dels mobles de l'hostaleria. Aquests mobles compten amb una gran
              personalització i exigència. Algunes qualitats del Contract són:
              Facilitat d'adaptació de l'estil i la decoració, Creació
              d'atmosferes més acollidores, Aportació d'atractiu visual als
              espais, Gran nivell de resistència i durabilitat, Oferta àmplia
              (models, colors…) i Perfecta connexió entre decoració,
              interiorisme i comoditat.
            </p>
            <div class="bg-light rounded p-4">
              <p class="text-muted font-italic mb-0">
                En Reformes Tarazona sabem, que en un disseny cada part del
                mateix compte tant com la suma de totes les seues parts.
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
                      Project Info :
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
              <h4 class="title mb-4">Projectes de Contract</h4>
              <p class="text-muted para-desc mx-auto mb-0">
                Comptem amb un àmplia experiència en el sector de les reformes,
                ací pots veure alguns dels nostres treballs ja realitzats.
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
