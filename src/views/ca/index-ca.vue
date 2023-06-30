<script>
import {
  ArrowUpIcon,
  ArrowRightIcon,
  FacebookIcon,
  InstagramIcon,
  TwitterIcon,
  LinkedinIcon,
} from "vue-feather-icons";

import Navbar from "@/components/ca/navbar";
// import Switcher from "@/components/switcher";
import Footer from "@/components/ca/footer";

/**
 * Index-seo-agency component
 */
export default {
  components: {
    Navbar,
    // Switcher,
    Footer,
    ArrowUpIcon,
    ArrowRightIcon,
    FacebookIcon,
    InstagramIcon,
    TwitterIcon,
    LinkedinIcon,
  },
  data() {
    return {
      list: [
        {
          image: "images/construction/o1.jpg",
          title: "Iphone mockup",
          type: "offices",
          category: "offices",
        },
        {
          image: "images/construction/b1.jpg",
          title: "Mockup Collection",
          type: "Mockup",
          category: "buildings",
        },
        {
          image: "images/construction/r1.jpg",
          title: "Abstract images",
          type: "Abstract",
          category: "roads",
        },
        {
          image: "images/construction/b2.jpg",
          title: "Yellow bg with Books",
          type: "Books",
          category: "buildings",
        },
        {
          image: "images/construction/r2.jpg",
          title: "Company V-card",
          type: "V-card",
          category: "roads",
        },
        {
          image: "images/construction/o2.jpg",
          title: "Mockup box with paints",
          type: "Photography",
          category: "offices",
        },
      ],
      filterCategory: "all",
      index: 0,
    };
  },
  mounted() {
    document
      .getElementById("color-opt")
      .setAttribute("href", "./css/colors/yellow.css");
  },
  destroyed() {
    document
      .getElementById("color-opt")
      .setAttribute("href", "./css/colors/default.css");
  },
  computed: {
    filteredData: function () {
      if (this.filterCategory === "all") {
        return this.list;
      } else {
        return this.list.filter((x) => x.category === this.filterCategory);
      }
    },
  },
  methods: {
    updateFilter(filterName) {
      this.filterCategory = filterName;
    },
  },
};
</script>

<template>
  <div>
    <Navbar :nav-light="true" />

    <!-- Hero Start -->
    <section
      class="bg-half-260 d-table w-100"
      style="background: url('images/principal/fondo.png') center center"
    >
      <div class="bg-overlay" style="opacity: 0.65"></div>
      <div class="container">
        <div class="row mt-5 mt-md-4">
          <div class="col-12">
            <div class="title-heading">
              <h1 class="display-4 mb-4 font-weight-bold text-white title-dark">
                Vols la teua
                <span class="text-primary font-weight-bold">casa</span><br />
                somniada?
              </h1>
              <p class="para-desc text-white-50">
                En Reformes Tarazona realitzem tot tipus de reformes, des de la
                teua cuina al teu bany, canviant taulells, parquet, mobles,
                mampares, etc.
              </p>
              <div class="mt-4 pt-2">
                <router-link to="/contacte" class="btn btn-primary"
                  >Contacta'ns</router-link
                >
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

    <section class="section bg-light">
      <div class="container">
        <div class="row">
          <div class="col-lg-12">
            <div class="features-absolute rounded bg-white shadow">
              <div class="row">
                <div class="col-lg-8 col-md-12 my-4">
                  <div class="row">
                    <div class="col-md-6 col-12">
                      <div class="media features p-4">
                        <div
                          class="icon text-center rounded-circle text-primary mr-3 mt-2"
                        >
                          <i
                            class="uil uil-shopping-bag align-middle h4 mb-0"
                          ></i>
                        </div>
                        <div class="media-body">
                          <h2 class="title">Venda de productes</h2>
                          <p class="text-muted para mb-0">
                            Gran varietat de productes i mobles per al bany, la
                            cuina i la llar.
                          </p>
                        </div>
                      </div>
                    </div>
                    <!--end col-->

                    <div class="col-md-6 col-12">
                      <div class="media features p-4">
                        <div
                          class="icon text-center rounded-circle text-primary mr-3 mt-2"
                        >
                          <i
                            class="uil uil-constructor align-middle h4 mb-0"
                          ></i>
                        </div>
                        <div class="media-body">
                          <h2 class="title">Reformes</h2>
                          <p class="text-muted para mb-0">
                            Reformes de les diferents zones de la teua casa,
                            tant d'interior com d'exterior.
                          </p>
                        </div>
                      </div>
                    </div>
                    <!--end col-->

                    <div class="col-md-6 col-12">
                      <div class="media features p-4">
                        <div
                          class="icon text-center rounded-circle text-primary mr-3 mt-2"
                        >
                          <i
                            class="uil uil-swatchbook align-middle h4 mb-0"
                          ></i>
                        </div>
                        <div class="media-body">
                          <h2 class="title">Contract</h2>
                          <p class="text-muted para mb-0">
                            Dissenys exclusius a mesura per a aconseguir
                            l'estada dels teus somnis.
                          </p>
                        </div>
                      </div>
                    </div>
                    <!--end col-->

                    <div class="col-md-6 col-12">
                      <div class="media features p-4">
                        <div
                          class="icon text-center rounded-circle text-primary mr-3 mt-2"
                        >
                          <i class="uil uil-selfie align-middle h4 mb-0"></i>
                        </div>
                        <div class="media-body">
                          <h2 class="title">Assessorament</h2>
                          <p class="text-muted para mb-0">
                            T'assessorem i aconsellem sobre com millorar la teua
                            casa.
                          </p>
                        </div>
                      </div>
                    </div>
                    <!--end col-->
                  </div>
                  <!--end row-->
                </div>
                <!--end col-->

                <div class="col-lg-4 d-none d-lg-block position-relative">
                  <img
                    src="images/principal/baño_1.png"
                    class="img-fluid mx-auto d-block construction-img"
                    style="border-radius: 10px 10px 0px 0px"
                    alt=""
                  />
                </div>
                <!--end col-->
              </div>
              <!--end row-->
            </div>
          </div>
          <!--end col-->

          <div class="col-12 mt-4 pt-2 text-center">
            <p class="text-muted mb-0">
              Si vols conéixer tots els nostres serveis.
              <router-link to="/servicios" class="text-primary h6"
                >Fes clic ací</router-link
              >, si tens qualsevol dubte t'assessorarem!
            </p>
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
      <!-- Features Start -->
      <div class="container-fluid mt-5 pt-2">
        <div class="row">
          <div class="col-md-4">
            <div
              class="py-5 rounded shadow"
              style="
                background: url('images/principal/cocina-banner.png') top center;
              "
            >
              <div class="p-4 banner">
                <h3>
                  Descomptes en <br />
                  Cuines
                </h3>
                <a
                  href="javascript:void(0)"
                  class="btn btn-sm btn-soft-primary mt-2"
                  >Més info.</a
                >
              </div>
            </div>
          </div>
          <!--end col-->

          <div class="col-md-4 mt-4 pt-2 mt-sm-0 pt-sm-0">
            <div
              class="py-5 rounded shadow"
              style="
                background: url('images/principal/baño-banner.png') top center;
              "
            >
              <div class="p-4 banner">
                <h3>
                  Descomptes en <br />
                  Banys
                </h3>
                <a
                  href="javascript:void(0)"
                  class="btn btn-sm btn-soft-primary mt-2"
                  style="color= yellow"
                  >Més info.</a
                >
              </div>
            </div>
          </div>
          <!--end col-->

          <div class="col-md-4 mt-4 pt-2 mt-sm-0 pt-sm-0">
            <div
              class="py-5 rounded shadow"
              style="
                background: url('images/principal/mampara-banner.png') top
                  center;
              "
            >
              <div class="p-4 banner">
                <h3>
                  Descomptes en <br />
                  Mampares
                </h3>
                <a
                  href="javascript:void(0)"
                  class="btn btn-sm btn-soft-primary mt-2"
                  >Més info.</a
                >
              </div>
            </div>
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
      <!-- Features End -->
    </section>
    <!--end section-->

    <section class="section">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-lg-5 col-md-6 col-12">
            <div class="position-relative">
              <img
                src="images/principal/baño.png"
                class="rounded img-fluid mx-auto d-block"
                alt=""
              />
            </div>
          </div>
          <!--end col-->

          <div class="col-lg-7 col-md-6 col-12 mt-4 mt-sm-0 pt-2 pt-sm-0">
            <div class="ml-lg-5 ml-md-4">
              <div class="section-title">
                <span class="badge badge-pill badge-soft-primary"
                  >Sobre nosaltres</span
                >
                <h2 class="title mt-3 mb-4">
                  El canvi que la teua llar es
                  <span class="text-primary">mereix</span>.
                </h2>
                <p class="text-muted para-desc mx-auto">
                  En
                  <span class="text-primary font-weight-bold"
                    >Reformes Tarazona</span
                  >
                  fem qualsevol tipus de reforma, així com instal·lació i venda
                  de mampares de bany, mobles de cuina i bany, venda de taulells
                  i paviment, instal·lació i venda de parquet, mampares de bany,
                  aixeteria, etc.
                </p>
                <p class="text-muted para-desc mx-auto mb-0">
                  És moment d'aconseguir el canvi en la teua llar que tant
                  desitjaves, reformem l'interior i exterior de la teua casa,
                  per a aconseguir una harmonia en els espais. Especialistes en
                  cuines i banys.
                </p>
                <br />
                <p class="text-muted para-desc mx-auto mb-0">
                  Si vols saber més sobre nosaltres pots veure els projectes que
                  hem realitzat des del següent enllaç.
                </p>
                <div class="mt-4">
                  <router-link to="/proyectos" class="btn btn-primary"
                    >Projectes</router-link
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

      <!-- Start CTA -->
      <div class="container-fluid mt-100 mt-60">
        <div
          class="rounded py-5"
          style="background: url('images/shop/cta.jpg') fixed"
        >
          <div class="container">
            <div class="row">
              <div class="col-12">
                <div class="section-title">
                  <h2 class="font-weight-bold mb-4">
                    Canvi de banyera per plat de dutxa <br />
                    Descompte del 30%
                  </h2>
                  <p class="para-desc para-white text-muted mb-0">
                    Cansat de fer esforços quan et dutxaràs? Pateixes de dolor
                    de genoll? En Reformes Tarazona tenim la solució! Canvia la
                    teua banyera per un modern plat de dutxa, veuràs el còmode i
                    fàcil que pot ser.
                  </p>
                  <div class="mt-4">
                    <a href="javascript:void(0)" class="btn btn-primary"
                      >Saber més</a
                    >
                  </div>
                </div>
              </div>
              <!--end col-->
            </div>
            <!--end row-->
          </div>
          <!--end container-->
        </div>
      </div>
      <!--end container-->
      <!-- End CTA -->

      <div class="container mt-100 mt-60">
        <div class="row">
          <div class="col-lg-4 col-md-6">
            <div class="section-title sticky-bar position-sticky">
              <span class="badge badge-pill badge-soft-primary">Projectes</span>
              <h2 class="title mt-3 mb-4">Els nostres projectes</h2>
              <p class="text-muted para-desc mb-0">
                En
                <span class="text-primary font-weight-bold"
                  >Reformes Tarazona</span
                >
                comptem amb gran experiència en el sector de la construcció i
                les reformes, especialistes en banys i cuines, ací tens alguns
                dels nostres projectes.
              </p>
              <div class="mt-4 d-none d-md-block">
                <router-link to="/proyectos" class="btn btn-soft-primary"
                  >Ver más<arrow-right-icon
                    class="fea icon-sm"
                  ></arrow-right-icon
                ></router-link>
              </div>
            </div>
          </div>
          <!--end col-->

          <div class="col-lg-8 col-md-6 mt-4 pt-2 mt-sm-0 pt-sm-0">
            <div class="row">
              <ul
                class="col container-filter list-unstyled categories-filter mb-0"
                id="filter"
              >
                <li class="list-inline-item">
                  <a
                    class="categories-name border d-block text-dark rounded"
                    @click="updateFilter('all')"
                    :class="{ active: filterCategory == 'all' }"
                    >Tots</a
                  >
                </li>
                <li class="list-inline-item">
                  <a
                    class="categories-name border d-block text-dark rounded"
                    data-filter=".offices"
                    @click="updateFilter('offices')"
                    :class="{ active: filterCategory == 'offices' }"
                    >Offices</a
                  >
                </li>
                <li class="list-inline-item">
                  <a
                    class="categories-name border d-block text-dark rounded"
                    data-filter=".buildings"
                    @click="updateFilter('buildings')"
                    :class="{ active: filterCategory == 'buildings' }"
                    >Buildings</a
                  >
                </li>
                <li class="list-inline-item">
                  <a
                    class="categories-name border d-block text-dark rounded"
                    data-filter=".roads"
                    @click="updateFilter('roads')"
                    :class="{ active: filterCategory == 'roads' }"
                    >Roads</a
                  >
                </li>
              </ul>
            </div>
            <!--end row-->

            <div class="row projects-wrapper">
              <div
                class="col-lg-6 col-12 mt-4 pt-2 offices"
                v-for="(item, index) in filteredData"
                :key="index"
              >
                <div
                  class="card border-0 work-container work-classic shadow overflow-hidden"
                >
                  <div class="card-body p-0">
                    <router-link to="/contract"
                      ><img
                        :src="item.image"
                        class="img-fluid work-image"
                        alt=""
                    /></router-link>
                    <div class="content p-4">
                      <h5 class="mb-0">
                        <router-link to="/contract" class="text-dark title">{{
                          item.title
                        }}</router-link>
                      </h5>
                      <h6 class="text-muted tag mb-0">{{ item.type }}</h6>
                    </div>
                  </div>
                </div>
              </div>
              <!--end col-->

              <div class="col-12 mt-4 pt-2">
                <div class="d-block d-md-none">
                  <a href="javascript:void(0)" class="btn btn-soft-primary"
                    >Veure més
                    <arrow-right-icon class="fea icon-sm"></arrow-right-icon
                  ></a>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!--end row-->
      </div>
      <!--end container-->
      <div class="container mt-100 mt-60">
        <div class="row align-items-center">
          <div class="col-lg-4 col-md-3">
            <p class="text-muted mb-0">
              Treballem amb gran varietat d'empreses i marques per a oferir
              serveis de qualitat.
            </p>
          </div>
          <!--end col-->

          <div class="col-lg-8 col-md-9 mt-4 pt-2 mt-sm-0 pt-sm-0">
            <div class="rounded shadow bg-light p-4">
              <div class="row justify-content-center">
                <div class="col-lg-3 col-md-3 col-6 text-center py-4">
                  <img
                    src="images/client/amazon.svg"
                    class="avatar avatar-ex-sm"
                    alt=""
                  />
                </div>
                <!--end col-->

                <div class="col-lg-3 col-md-3 col-6 text-center py-4">
                  <img
                    src="images/client/google.svg"
                    class="avatar avatar-ex-sm"
                    alt=""
                  />
                </div>
                <!--end col-->

                <div class="col-lg-3 col-md-3 col-6 text-center py-4">
                  <img
                    src="images/client/lenovo.svg"
                    class="avatar avatar-ex-sm"
                    alt=""
                  />
                </div>
                <!--end col-->

                <div class="col-lg-3 col-md-3 col-6 text-center py-4">
                  <img
                    src="images/client/paypal.svg"
                    class="avatar avatar-ex-sm"
                    alt=""
                  />
                </div>
                <!--end col-->
              </div>
              <!--end row-->
            </div>
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </section>
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

<style>
.modal-content {
  background-color: transparent;
}
</style>
