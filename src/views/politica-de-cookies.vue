<script>
import { ArrowUpIcon, ArrowRightIcon } from "vue-feather-icons";

import Navbar from "@/components/navbar";
// import Switcher from "@/components/switcher";
import Footer from "@/components/footer";
/**
 * politica-de-cookies component
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
    ArrowRightIcon,
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
              <h1 class="title">Política de Cookies</h1>
              <div class="page-next">
                <nav aria-label="breadcrumb" class="d-inline-block">
                  <ul class="breadcrumb bg-white rounded shadow mb-0">
                    <li class="breadcrumb-item">
                      <router-link to="/">Inicio</router-link>
                    </li>
                    <li class="breadcrumb-item active" aria-current="page">
                      Política de Cookies
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

    <!-- Start Terms & Conditions -->
    <section class="section">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-lg-9">
            <div class="card shadow border-0 rounded">
              <div class="card-body">
                <h5 class="card-title">Introduction :</h5>
                <p class="text-muted">
                  It seems that only fragments of the original text remain in
                  the Lorem Ipsum texts used today. One may speculate that over
                  the course of time certain letters were added or deleted at
                  various positions within the text.
                </p>

                <h5 class="card-title">User Agreements :</h5>
                <p class="text-muted">
                  The most well-known dummy text is the 'Lorem Ipsum', which is
                  said to have <b class="text-danger">originated</b> in the 16th
                  century. Lorem Ipsum is <b class="text-danger">composed</b> in
                  a pseudo-Latin language which more or less
                  <b class="text-danger">corresponds</b> to 'proper' Latin. It
                  contains a series of real Latin words. This ancient dummy text
                  is also <b class="text-danger">incomprehensible</b>, but it
                  imitates the rhythm of most European languages in Latin
                  script. The <b class="text-danger">advantage</b> of its Latin
                  origin and the relative
                  <b class="text-danger">meaninglessness</b> of Lorum Ipsum is
                  that the text does not attract attention to itself or distract
                  the viewer's <b class="text-danger">attention</b> from the
                  layout.
                </p>
                <p class="text-muted">
                  There is now an <b class="text-danger">abundance</b> of
                  readable dummy texts. These are usually used when a text is
                  <b class="text-danger">required purely</b> to fill a space.
                  These alternatives to the classic Lorem Ipsum texts are often
                  amusing and tell short, funny or
                  <b class="text-danger">nonsensical</b> stories.
                </p>
                <p class="text-muted">
                  It seems that only <b class="text-danger">fragments</b> of the
                  original text remain in the Lorem Ipsum texts used today. One
                  may speculate that over the course of time certain letters
                  were added or deleted at various positions within the text.
                </p>

                <h5 class="card-title">Restrictions :</h5>
                <p class="text-muted">
                  You are specifically restricted from all of the following :
                </p>
                <ul class="list-unstyled text-muted">
                  <li>
                    <arrow-right-icon
                      class="fea icon-sm mr-2"
                    ></arrow-right-icon
                    >Digital Marketing Solutions for Tomorrow
                  </li>
                  <li>
                    <arrow-right-icon
                      class="fea icon-sm mr-2"
                    ></arrow-right-icon
                    >Our Talented & Experienced Marketing Agency
                  </li>
                  <li>
                    <arrow-right-icon
                      class="fea icon-sm mr-2"
                    ></arrow-right-icon
                    >Create your own skin to match your brand
                  </li>
                  <li>
                    <arrow-right-icon
                      class="fea icon-sm mr-2"
                    ></arrow-right-icon
                    >Digital Marketing Solutions for Tomorrow
                  </li>
                  <li>
                    <arrow-right-icon
                      class="fea icon-sm mr-2"
                    ></arrow-right-icon
                    >Our Talented & Experienced Marketing Agency
                  </li>
                  <li>
                    <arrow-right-icon
                      class="fea icon-sm mr-2"
                    ></arrow-right-icon
                    >Create your own skin to match your brand
                  </li>
                </ul>

                <h5 class="card-title">Users Question & Answer :</h5>
                <div class="faq-content mt-4">
                  <div class="accordion" id="accordionExampleone">
                    <b-card no-body class="mb-2 border-0 rounded">
                      <b-card-header class="border-0 bg-light p-3 pr-5">
                        <a
                          class="faq position-relative text-dark"
                          v-b-toggle.accordion-1
                          href="javascript: void(0);"
                        >
                          <h6 class="title mb-0">
                            How our<span class="text-primary"> Landrick</span>
                            work ?
                          </h6>
                        </a>
                      </b-card-header>
                      <b-collapse
                        id="accordion-1"
                        visible
                        accordion="my-accordion"
                        role="tabpanel"
                      >
                        <b-card-body class="px-2 py-4">
                          <p class="text-muted mb-0 faq-ans">
                            There are many variations of passages of Lorem Ipsum
                            available, but the majority have suffered alteration
                            in some form.
                          </p>
                        </b-card-body>
                      </b-collapse>
                    </b-card>
                    <b-card no-body class="mb-2 border-0 rounded">
                      <b-card-header class="border-0 bg-light p-3 pr-5">
                        <a
                          class="faq position-relative text-dark"
                          v-b-toggle.accordion-2
                          href="javascript: void(0);"
                        >
                          <h6 class="title mb-0">
                            What is the main process open account ?
                          </h6>
                        </a>
                      </b-card-header>
                      <b-collapse
                        id="accordion-2"
                        accordion="my-accordion"
                        role="tabpanel"
                      >
                        <b-card-body class="px-2 py-4">
                          <p class="text-muted mb-0 faq-ans">
                            There are many variations of passages of Lorem Ipsum
                            available, but the majority have suffered alteration
                            in some form.
                          </p>
                        </b-card-body>
                      </b-collapse>
                    </b-card>
                    <b-card no-body class="mb-2 border-0 rounded">
                      <b-card-header class="border-0 bg-light p-3 pr-5">
                        <a
                          class="faq position-relative text-dark"
                          v-b-toggle.accordion-3
                          href="javascript: void(0);"
                        >
                          <h6 class="title mb-0">
                            How to make unlimited data entry ?
                          </h6>
                        </a>
                      </b-card-header>
                      <b-collapse
                        id="accordion-3"
                        accordion="my-accordion"
                        role="tabpanel"
                      >
                        <b-card-body class="px-2 py-4">
                          <p class="text-muted mb-0 faq-ans">
                            There are many variations of passages of Lorem Ipsum
                            available, but the majority have suffered alteration
                            in some form.
                          </p>
                        </b-card-body>
                      </b-collapse>
                    </b-card>
                    <b-card no-body class="mb-2 border-0 rounded">
                      <b-card-header class="border-0 bg-light p-3 pr-5">
                        <a
                          class="faq position-relative text-dark"
                          v-b-toggle.accordion-4
                          href="javascript: void(0);"
                        >
                          <h6 class="title mb-0">
                            Is <span class="text-primary">Landrick</span> safer
                            to use with my account ?
                          </h6>
                        </a>
                      </b-card-header>
                      <b-collapse
                        id="accordion-4"
                        accordion="my-accordion"
                        role="tabpanel"
                      >
                        <b-card-body class="px-2 py-4">
                          <p class="text-muted mb-0 faq-ans">
                            There are many variations of passages of Lorem Ipsum
                            available, but the majority have suffered alteration
                            in some form.
                          </p>
                        </b-card-body>
                      </b-collapse>
                    </b-card>
                    <b-card no-body class="mb-2 border-0 rounded">
                      <b-card-header class="border-0 bg-light p-3 pr-5">
                        <a
                          class="faq position-relative text-dark"
                          v-b-toggle.accordion-5
                          href="javascript: void(0);"
                        >
                          <h6 class="title mb-0">
                            How can i contact your technical team ?
                          </h6>
                        </a>
                      </b-card-header>
                      <b-collapse
                        id="accordion-5"
                        accordion="my-accordion"
                        role="tabpanel"
                      >
                        <b-card-body class="px-2 py-4">
                          <p class="text-muted mb-0 faq-ans">
                            There are many variations of passages of Lorem Ipsum
                            available, but the majority have suffered alteration
                            in some form.
                          </p>
                        </b-card-body>
                      </b-collapse>
                    </b-card>
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
    </section>
    <!--end section-->
    <!-- End Terms & Conditions -->
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
