<script>
import { ArrowUpIcon } from "vue-feather-icons";

import Navbar from "@/components/navbar";
// import Switcher from "@/components/switcher";
import Footer from "@/components/footer";

/**
 * Page-work-classic component
 */
export default {
  data() {
    return {
      workData: [
        {
          image: "images/work/4.jpg",
          title: "Grifería",
          type: "Cocina",
          category: "cocina",
          url: "/src/views/shop-product-detail.vue",
        },
        {
          image: "images/work/4.jpg",
          title: "Muebles cocina",
          type: "Cocina",
          category: "cocina",
        },
        {
          image: "images/work/4.jpg",
          title: "Electrodomésticos",
          type: "Cocina",
          category: "cocina",
        },
        {
          image: "images/work/4.jpg",
          title: "Encimeras",
          type: "Cocina",
          category: "cocina",
        },
        {
          image: "images/work/4.jpg",
          title: "Accesorios",
          type: "Cocina",
          category: "cocina",
        },
        {
          image: "images/work/2.jpg",
          title: "Saneamiento",
          type: "Baño",
          category: "baño",
        },
        {
          image: "images/work/2.jpg",
          title: "Grifería",
          type: "Baño",
          category: "baño",
        },
        {
          image: "images/work/2.jpg",
          title: "Bañeras",
          type: "Baño",
          category: "baño",
        },
        {
          image: "images/work/2.jpg",
          title: "Duchas",
          type: "Baño",
          category: "baño",
        },
        {
          image: "images/work/2.jpg",
          title: "Mobiliario baño",
          type: "Baño",
          category: "baño",
        },
        {
          image: "images/work/2.jpg",
          title: "Mamparas",
          type: "Baño",
          category: "baño",
        },
        {
          image: "images/work/2.jpg",
          title: "Accesorios",
          type: "Baño",
          category: "baño",
        },
        {
          image: "images/work/3.jpg",
          title: "Porcelánico",
          type: "Suelos",
          category: "suelos",
        },
        {
          image: "images/work/3.jpg",
          title: "Parquet",
          type: "Suelos",
          category: "suelos",
        },
        {
          image: "images/work/3.jpg",
          title: "Laminado",
          type: "Suelos",
          category: "suelos",
        },
        {
          image: "images/work/3.jpg",
          title: "Vinílico",
          type: "Suelos",
          category: "suelos",
        },
        {
          image: "images/work/3.jpg",
          title: "Exterior",
          type: "Suelos",
          category: "suelos",
        },
        {
          image: "images/work/3.jpg",
          title: "Moqueta",
          type: "Suelos",
          category: "suelos",
        },
        {
          image: "images/work/4.jpg",
          title: "Puertas de entrada y exterior",
          type: "Puertas",
          category: "puertas",
        },
        {
          image: "images/work/4.jpg",
          title: "Puertas de interior",
          type: "Puertas",
          category: "puertas",
        },
        {
          image: "images/work/6.jpg",
          title: "Aluminio",
          type: "Ventanas",
          category: "ventanas",
        },
        {
          image: "images/work/6.jpg",
          title: "PVC",
          type: "Ventanas",
          category: "ventanas",
        },
        {
          image: "images/work/6.jpg",
          title: "Ventanas a medida",
          type: "Ventanas",
          category: "ventanas",
        },
        {
          image: "images/work/6.jpg",
          title: "Ventanas de techo y Claraboyas",
          type: "Ventanas",
          category: "ventanas",
        },
        {
          image: "images/work/6.jpg",
          title: "Mosquiteras",
          type: "Ventanas",
          category: "ventanas",
        },
      ],
      filterCategory: "all",
    };
  },
  components: {
    Navbar,
    // Switcher,
    Footer,
    ArrowUpIcon,
  },
  computed: {
    filteredData: function () {
      if (this.filterCategory === "all") {
        return this.workData;
      } else {
        return this.workData.filter((x) => x.category === this.filterCategory);
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
    <Navbar />

    <!-- Hero Start -->
    <section class="bg-half bg-light d-table w-100">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-lg-12 text-center">
            <div class="page-next-level">
              <h1 class="title">Productos</h1>
              <div class="page-next">
                <nav aria-label="breadcrumb" class="d-inline-block">
                  <ul class="breadcrumb bg-white rounded shadow mb-0">
                    <li class="breadcrumb-item">
                      <router-link to="/">Inicio</router-link>
                    </li>
                    <li class="breadcrumb-item active" aria-current="page">
                      Productos
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

    <!-- Start -->
    <section class="section">
      <div class="container">
        <div class="row">
          <ul
            class="col container-filter list-unstyled categories-filter text-center mb-0"
            id="filter"
          >
            <li class="list-inline-item">
              <a
                class="categories border d-block text-dark rounded"
                @click="updateFilter('all')"
                :class="{ active: filterCategory == 'all' }"
                >Todos</a
              >
            </li>
            <li class="list-inline-item">
              <a
                class="categories border d-block text-dark rounded"
                @click="updateFilter('cocina')"
                :class="{ active: filterCategory == 'cocina' }"
                >Cocina</a
              >
            </li>
            <li class="list-inline-item">
              <a
                class="categories border d-block text-dark rounded"
                @click="updateFilter('baño')"
                :class="{ active: filterCategory == 'baño' }"
                >Baño</a
              >
            </li>
            <li class="list-inline-item">
              <a
                class="categories border d-block text-dark rounded"
                @click="updateFilter('suelos')"
                :class="{ active: filterCategory == 'suelos' }"
                >Suelos</a
              >
            </li>
            <li class="list-inline-item">
              <a
                class="categories border d-block text-dark rounded"
                @click="updateFilter('puertas')"
                :class="{ active: filterCategory == 'puertas' }"
                >Puertas</a
              >
            </li>
            <li class="list-inline-item">
              <a
                class="categories border d-block text-dark rounded"
                @click="updateFilter('ventanas')"
                :class="{ active: filterCategory == 'ventanas' }"
                >Ventanas</a
              >
            </li>
          </ul>
        </div>
        <!--end row-->

        <div class="row projects-wrapper">
          <div
            class="col-lg-4 col-md-6 col-12 mt-4 pt-2 branding"
            v-for="(item, index) in filteredData"
            :key="index"
          >
            <div class="card border-0 work-container work-classic">
              <div class="card-body p-0">
                <router-link to="/page-blog-grid"
                  ><img
                    :src="item.image"
                    class="img-fluid rounded work-image"
                    alt=""
                /></router-link>
                <div class="content pt-3">
                  <h5 class="mb-0">
                    <router-link to="/page-blog-grid" class="text-dark title">{{
                      item.title
                    }}</router-link>
                  </h5>
                  <h6 class="text-muted tag mb-0">{{ item.type }}</h6>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!--end row-->
      </div>
      <!--end container-->
    </section>
    <!--end section-->
    <!-- End -->
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
