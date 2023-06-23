<script>
import { ArrowUpIcon } from "vue-feather-icons";

import Navbar from "@/components/navbar";
import Switcher from "@/components/switcher";
import Footer from "@/components/footer";

/**
 * Page-blog-grid component
 */
export default {
  data() {
    return {};
  },
  components: {
    Navbar,
    Switcher,
    Footer,
    ArrowUpIcon,
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
              <h1 class="title">Grifería</h1>
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
                      Grifería
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

    <!-- Blog STart -->
    <section class="section">
      <div class="container">
        <div class="row">
          <div class="col-lg-4 col-md-6 mb-4 pb-2">
            <div class="card blog rounded border-0 shadow overflow-hidden">
              <div class="position-relative">
                <img
                  src="images/productos/sub-griferia-1.png"
                  class="card-img-top"
                  alt="..."
                />
                <div class="overlay rounded-top bg-dark"></div>
              </div>
              <div class="card-body content">
                <h5>
                  <a
                    href="/shop-product-detail"
                    class="card-title title text-dark"
                    >Grifo modelo 1</a
                  >
                </h5>
                <div class="post-meta d-flex justify-content-between mt-3">
                  <router-link
                    to="/shop-product-detail"
                    class="text-muted readmore"
                    >Saber más <i class="mdi mdi-chevron-right"></i
                  ></router-link>
                </div>
              </div>
            </div>
          </div>
          <!--end col-->

          <div class="col-lg-4 col-md-6 mb-4 pb-2">
            <div class="card blog rounded border-0 shadow overflow-hidden">
              <div class="position-relative">
                <img
                  src="images/productos/sub-griferia-2.png"
                  class="card-img-top"
                  alt="..."
                />
                <div class="overlay rounded-top bg-dark"></div>
              </div>
              <div class="card-body content">
                <h5>
                  <a
                    href="javascript:void(0)"
                    class="card-title title text-dark"
                    >Grifo modelo 2</a
                  >
                </h5>
                <div class="post-meta d-flex justify-content-between mt-3">
                  <router-link
                    to="/page-blog-detail"
                    class="text-muted readmore"
                    >Saber más <i class="mdi mdi-chevron-right"></i
                  ></router-link>
                </div>
              </div>
            </div>
          </div>
          <!--end col-->

          <div class="col-lg-4 col-md-6 mb-4 pb-2">
            <div class="card blog rounded border-0 shadow overflow-hidden">
              <div class="position-relative">
                <img
                  src="images/productos/sub-griferia-3.png"
                  class="card-img-top"
                  alt="..."
                />
                <div class="overlay rounded-top bg-dark"></div>
              </div>
              <div class="card-body content">
                <h5>
                  <a
                    href="javascript:void(0)"
                    class="card-title title text-dark"
                    >Grifo modelo 3</a
                  >
                </h5>
                <div class="post-meta d-flex justify-content-between mt-3">
                  <router-link
                    to="/page-blog-detail"
                    class="text-muted readmore"
                    >Saber más <i class="mdi mdi-chevron-right"></i
                  ></router-link>
                </div>
              </div>
            </div>
          </div>
          <!--end col-->

          <div class="col-lg-4 col-md-6 mb-4 pb-2">
            <div class="card blog rounded border-0 shadow overflow-hidden">
              <div class="position-relative">
                <img
                  src="images/productos/sub-griferia-4.png"
                  class="card-img-top"
                  alt="..."
                />
                <div class="overlay rounded-top bg-dark"></div>
              </div>
              <div class="card-body content">
                <h5>
                  <a
                    href="javascript:void(0)"
                    class="card-title title text-dark"
                    >Grifo modelo 4</a
                  >
                </h5>
                <div class="post-meta d-flex justify-content-between mt-3">
                  <router-link
                    to="/page-blog-detail"
                    class="text-muted readmore"
                    >Saber más <i class="mdi mdi-chevron-right"></i
                  ></router-link>
                </div>
              </div>
            </div>
          </div>
          <!--end col-->

          <div class="col-lg-4 col-md-6 mb-4 pb-2">
            <div class="card blog rounded border-0 shadow overflow-hidden">
              <div class="position-relative">
                <img
                  src="images/productos/sub-griferia-5.png"
                  class="card-img-top"
                  alt="..."
                />
                <div class="overlay rounded-top bg-dark"></div>
              </div>
              <div class="card-body content">
                <h5>
                  <a
                    href="javascript:void(0)"
                    class="card-title title text-dark"
                    >Grifo modelo 5</a
                  >
                </h5>
                <div class="post-meta d-flex justify-content-between mt-3">
                  <router-link
                    to="/shop-product-detail"
                    class="text-muted readmore"
                    >Saber más <i class="mdi mdi-chevron-right"></i
                  ></router-link>
                </div>
              </div>
            </div>
          </div>
          <!--end col-->

          <!-- PAGINATION START -->
          <div class="col-12">
            <ul class="pagination justify-content-center mb-0">
              <li class="page-item">
                <a
                  class="page-link"
                  href="javascript:void(0)"
                  aria-label="Previous"
                  >Ant</a
                >
              </li>
              <li class="page-item active">
                <a class="page-link" href="javascript:void(0)">1</a>
              </li>
              <li class="page-item">
                <a class="page-link" href="javascript:void(0)">2</a>
              </li>
              <li class="page-item">
                <a class="page-link" href="javascript:void(0)">3</a>
              </li>
              <li class="page-item">
                <a class="page-link" href="javascript:void(0)" aria-label="Next"
                  >Sig</a
                >
              </li>
            </ul>
          </div>
          <!--end col-->
          <!-- PAGINATION END -->
        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </section>
    <!--end section-->
    <!-- Blog End -->
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
