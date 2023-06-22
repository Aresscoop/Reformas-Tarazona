<script>
import {
  ArrowUpIcon,
  HeartIcon,
  EyeIcon,
  ShoppingCartIcon,
  MessageCircleIcon,
  MailIcon,
  UserIcon,
} from "vue-feather-icons";
import { Carousel, Slide } from "vue-carousel";
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
import Navbar from "@/components/navbar";
// import Switcher from "@/components/switcher";
import Footer from "@/components/footer";

/**
 * Shop-product-detail component
 */
export default {
  data() {
    return {
      countval: 1,
    };
  },
  components: {
    Navbar,
    // Switcher,
    Footer,
    Carousel,
    Slide,
    ArrowUpIcon,
    VueSlickCarousel,
    HeartIcon,
    EyeIcon,
    ShoppingCartIcon,
    MessageCircleIcon,
    MailIcon,
    UserIcon,
  },
  methods: {
    increment() {
      this.countval++;
    },
    decrement() {
      if (this.countval > 0) this.countval--;
    },
  },
};
</script>

<template>
  <div>
    <Navbar :isIcons="true" />

    <!-- Hero Start -->
    <section class="bg-half bg-light d-table w-100">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-lg-12 text-center">
            <div class="page-next-level">
              <h1 class="title">Nombre Producto</h1>
              <div class="page-next">
                <nav aria-label="breadcrumb" class="d-inline-block">
                  <ul class="breadcrumb bg-white rounded shadow mb-0">
                    <li class="breadcrumb-item">
                      <router-link to="/">Inicio</router-link>
                    </li>
                    <li class="breadcrumb-item">
                      <router-link to="/productos">Productos</router-link>
                    </li>
                    <li class="breadcrumb-item active" aria-current="page">
                      Categoría
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
    <!-- Hero End -->

    <section class="section">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-md-5">
            <VueSlickCarousel
              ref="c1"
              :arrows="false"
              :focusOnSelect="true"
              :asNavFor="$refs.c2"
              :dots="false"
              :autoplay="true"
              :fade="true"
            >
              <div>
                <img
                  src="images/shop/product/single-2.jpg"
                  class="img-fluid rounded"
                  alt=""
                />
              </div>
              <div>
                <img
                  src="images/shop/product/single-3.jpg"
                  class="img-fluid rounded"
                  alt=""
                />
              </div>
              <div>
                <img
                  src="images/shop/product/single-4.jpg"
                  class="img-fluid rounded"
                  alt=""
                />
              </div>
              <div>
                <img
                  src="images/shop/product/single-5.jpg"
                  class="img-fluid rounded"
                  alt=""
                />
              </div>
              <div>
                <img
                  src="images/shop/product/single-6.jpg"
                  class="img-fluid rounded"
                  alt=""
                />
              </div>
              <div>
                <img
                  src="images/shop/product/single-3.jpg"
                  class="img-fluid rounded"
                  alt=""
                />
              </div>
            </VueSlickCarousel>

            <VueSlickCarousel
              :asNavFor="$refs.c1"
              :arrows="false"
              :focusOnSelect="true"
              ref="c2"
              class="slick-slide"
              :slidesToShow="3"
            >
              <div>
                <img
                  src="images/shop/product/single-2.jpg"
                  class="img-fluid"
                  alt=""
                />
              </div>
              <div>
                <img
                  src="images/shop/product/single-3.jpg"
                  class="img-fluid"
                  alt=""
                />
              </div>
              <div>
                <img
                  src="images/shop/product/single-4.jpg"
                  class="img-fluid"
                  alt=""
                />
              </div>
              <div>
                <img
                  src="images/shop/product/single-5.jpg"
                  class="img-fluid"
                  alt=""
                />
              </div>
              <div>
                <img
                  src="images/shop/product/single-6.jpg"
                  class="img-fluid"
                  alt=""
                />
              </div>
              <div>
                <img
                  src="images/shop/product/single-3.jpg"
                  class="img-fluid"
                  alt=""
                />
              </div>
            </VueSlickCarousel>
          </div>
          <!--end col-->

          <div class="col-md-7 mt-4 mt-sm-0 pt-2 pt-sm-0">
            <div class="section-title ml-md-4">
              <h2 class="title">Nombre del Producto</h2>
              <p class="text-muted">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero
                exercitationem, unde molestiae sint quae inventore atque minima
                natus fugiat nihil quisquam voluptates ea omnis. Modi laborum
                soluta tempore unde accusantium.
              </p>

              <ul class="list-unstyled text-muted">
                <li class="mb-0">
                  <span class="text-primary h5 mr-2"
                    ><i class="uil uil-check-circle align-middle"></i
                  ></span>
                  Digital Marketing Solutions for Tomorrow
                </li>
                <li class="mb-0">
                  <span class="text-primary h5 mr-2"
                    ><i class="uil uil-check-circle align-middle"></i
                  ></span>
                  Our Talented &amp; Experienced Marketing Agency
                </li>
                <li class="mb-0">
                  <span class="text-primary h5 mr-2"
                    ><i class="uil uil-check-circle align-middle"></i
                  ></span>
                  Create your own skin to match your brand
                </li>
              </ul>
              <!--end row-->
              <div class="container mt-100 mt-5">
                <div class="row">
                  <div class="col-12">
                    <b-tabs
                      content-class="mt-5"
                      pills
                      nav-class="bg-white shadow"
                    >
                      <b-tab active title-item-class="m-1">
                        <template #title>
                          <span class="nav-link py-2 px-5">
                            <div class="text-center">
                              <h6 class="mb-0">Descripción</h6>
                            </div></span
                          >
                        </template>

                        <p class="text-muted mb-0">
                          Due to its widespread use as filler text for layouts,
                          non-readability is of great importance: human
                          perception is tuned to recognize certain patterns and
                          repetitions in texts. If the distribution of letters
                          and 'words' is random, the reader will not be
                          distracted from making a neutral judgement on the
                          visual impact and readability of the typefaces
                          (typography), or the distribution of text on the page
                          (layout or type area). For this reason, dummy text
                          usually consists of a more or less random series of
                          words or syllables.
                        </p>
                      </b-tab>
                      <b-tab title-item-class="m-1">
                        <template #title>
                          <span class="nav-link py-2 px-5 rounded">
                            <div class="text-center">
                              <h6 class="mb-0">Información técnica</h6>
                            </div>
                          </span>
                        </template>
                        <table class="table">
                          <tbody>
                            <tr>
                              <td style="width: 100px">Color</td>
                              <td class="text-muted">
                                Red, White, Black, Orange
                              </td>
                            </tr>

                            <tr>
                              <td>Material</td>
                              <td class="text-muted">Cotton</td>
                            </tr>

                            <tr>
                              <td>Size</td>
                              <td class="text-muted">S, M, L, XL, XXL</td>
                            </tr>
                          </tbody>
                        </table>
                      </b-tab>
                    </b-tabs>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->

      <div class="container mt-100 mt-60">
        <div class="row">
          <div class="col-12">
            <h5 class="mb-0">Productos Relacionados</h5>
          </div>
          <!--end col-->

          <div class="col-12 mt-4">
            <carousel
              id="client-four"
              class="owl-carousel owl-theme"
              dir="ltr"
              :per-page="3"
              :loop="true"
            >
              <Slide>
                <div
                  class="card shop-list border-0 position-relative overflow-hidden m-2"
                >
                  <div
                    class="shop-image position-relative overflow-hidden rounded shadow"
                  >
                    <router-link to="/shop-product-detail"
                      ><img
                        src="images/shop/product/s1.jpg"
                        class="img-fluid"
                        alt=""
                    /></router-link>
                    <router-link to="/shop-product-detail" class="overlay-work">
                      <img
                        src="images/shop/product/s-1.jpg"
                        class="img-fluid"
                        alt=""
                      />
                    </router-link>
                    <ul class="list-unstyled shop-icons">
                      <li>
                        <a
                          href="javascript:void(0)"
                          class="btn btn-icon btn-pills btn-soft-danger"
                        >
                          <heart-icon class="icons"></heart-icon>
                        </a>
                      </li>
                      <li class="mt-2">
                        <a
                          href="shop-product-detail"
                          class="btn btn-icon btn-pills btn-soft-primary"
                        >
                          <eye-icon class="icons"></eye-icon>
                        </a>
                      </li>
                    </ul>
                  </div>
                  <div class="card-body content pt-4 p-2">
                    <router-link
                      to="/shop-product-detail"
                      class="text-dark product-name h6"
                      >Branded T-Shirt</router-link
                    >
                  </div>
                </div>
              </Slide>
              <Slide>
                <div
                  class="card shop-list border-0 position-relative overflow-hidden m-2"
                >
                  <div
                    class="shop-image position-relative overflow-hidden rounded shadow"
                  >
                    <router-link to="/shop-product-detail"
                      ><img
                        src="images/shop/product/s3.jpg"
                        class="img-fluid"
                        alt=""
                    /></router-link>
                    <router-link to="/shop-product-detail" class="overlay-work">
                      <img
                        src="images/shop/product/s-3.jpg"
                        class="img-fluid"
                        alt=""
                      />
                    </router-link>
                    <ul class="list-unstyled shop-icons">
                      <li>
                        <a
                          href="javascript:void(0)"
                          class="btn btn-icon btn-pills btn-soft-danger"
                        >
                          <heart-icon class="icons"></heart-icon>
                        </a>
                      </li>
                      <li class="mt-2">
                        <a
                          href="shop-product-detail"
                          class="btn btn-icon btn-pills btn-soft-primary"
                        >
                          <eye-icon class="icons"></eye-icon>
                        </a>
                      </li>
                    </ul>
                  </div>
                  <div class="card-body content pt-4 p-2">
                    <router-link
                      to="/shop-product-detail"
                      class="text-dark product-name h6"
                      >Elegent Watch</router-link
                    >
                  </div>
                </div>
              </Slide>
              <Slide>
                <div
                  class="card shop-list border-0 position-relative overflow-hidden m-2"
                >
                  <div
                    class="shop-image position-relative overflow-hidden rounded shadow"
                  >
                    <router-link to="/shop-product-detail"
                      ><img
                        src="images/shop/product/s6.jpg"
                        class="img-fluid"
                        alt=""
                    /></router-link>
                    <router-link to="/shop-product-detail" class="overlay-work">
                      <img
                        src="images/shop/product/s-6.jpg"
                        class="img-fluid"
                        alt=""
                      />
                    </router-link>
                    <ul class="list-unstyled shop-icons">
                      <li>
                        <a
                          href="javascript:void(0)"
                          class="btn btn-icon btn-pills btn-soft-danger"
                        >
                          <heart-icon class="icons"></heart-icon>
                        </a>
                      </li>
                      <li class="mt-2">
                        <a
                          href="shop-product-detail"
                          class="btn btn-icon btn-pills btn-soft-primary"
                        >
                          <eye-icon class="icons"></eye-icon>
                        </a>
                      </li>
                    </ul>
                  </div>
                  <div class="card-body content pt-4 p-2">
                    <router-link
                      to="/shop-product-detail"
                      class="text-dark product-name h6"
                      >Elegent Mug</router-link
                    >
                  </div>
                </div>
              </Slide>
              <Slide>
                <div
                  class="card shop-list border-0 position-relative overflow-hidden m-2"
                >
                  <div
                    class="shop-image position-relative overflow-hidden rounded shadow"
                  >
                    <router-link to="/shop-product-detail"
                      ><img
                        src="images/shop/product/s8.jpg"
                        class="img-fluid"
                        alt=""
                    /></router-link>
                    <router-link to="/shop-product-detail" class="overlay-work">
                      <img
                        src="images/shop/product/s-8.jpg"
                        class="img-fluid"
                        alt=""
                      />
                    </router-link>
                    <ul class="list-unstyled shop-icons">
                      <li>
                        <a
                          href="javascript:void(0)"
                          class="btn btn-icon btn-pills btn-soft-danger"
                        >
                          <heart-icon class="icons"></heart-icon>
                        </a>
                      </li>
                      <li class="mt-2">
                        <router-link
                          to="/shop-product-detail"
                          class="btn btn-icon btn-pills btn-soft-primary"
                        >
                          <eye-icon class="icons"></eye-icon>
                        </router-link>
                      </li>
                    </ul>
                  </div>
                  <div class="card-body content pt-4 p-2">
                    <router-link
                      to="/shop-product-detail"
                      class="text-dark product-name h6"
                      >Wooden Stools</router-link
                    >
                  </div>
                </div>
              </Slide>
              <Slide>
                <div
                  class="card shop-list border-0 position-relative overflow-hidden m-2"
                >
                  <div
                    class="shop-image position-relative overflow-hidden rounded shadow"
                  >
                    <router-link to="/shop-product-detail"
                      ><img
                        src="images/shop/product/s14.jpg"
                        class="img-fluid"
                        alt=""
                    /></router-link>
                    <router-link to="/shop-product-detail" class="overlay-work">
                      <img
                        src="images/shop/product/s-14.jpg"
                        class="img-fluid"
                        alt=""
                      />
                    </router-link>
                    <ul class="list-unstyled shop-icons">
                      <li>
                        <a
                          href="javascript:void(0)"
                          class="btn btn-icon btn-pills btn-soft-danger"
                        >
                          <heart-icon class="icons"></heart-icon>
                        </a>
                      </li>
                      <li class="mt-2">
                        <router-link
                          to="/shop-product-detail"
                          class="btn btn-icon btn-pills btn-soft-primary"
                        >
                          <eye-icon class="icons"></eye-icon>
                        </router-link>
                      </li>
                    </ul>
                  </div>
                  <div class="card-body content pt-4 p-2">
                    <router-link
                      to="/shop-product-detail"
                      class="text-dark product-name h6"
                      >Women Block Heels</router-link
                    >
                  </div>
                </div>
              </Slide>
            </carousel>
          </div>
          <!--end col-->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </section>
    <!--end section-->
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
