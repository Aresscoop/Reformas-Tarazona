<script>
import { ArrowUpIcon } from "vue-feather-icons";
import { Carousel, Slide } from "vue-carousel";

import Navbar from "@/components/navbar";
// import Switcher from "@/components/switcher";
import Footer from "@/components/footer";

/**
 * Shop-cart component
 */
export default {
  data() {
    return {
      counter: 0,
      list: [
        {
          id: 1,
          image: "images/shop/product/s1.jpg",
          title: "T-Shirt",
          price: 255,
          qty: 2,
          total: 510,
        },
        {
          id: 2,
          image: "images/shop/product/s3.jpg",
          title: "Branded Watch",
          price: 520,
          qty: 1,
          total: 520,
        },
        {
          id: 3,
          image: "images/shop/product/s6.jpg",
          title: "T-Shirt",
          price: 160,
          qty: 4,
          total: 640,
        },
        {
          id: 4,
          image: "images/shop/product/s10.jpg",
          title: "Branded Watch",
          price: 260,
          qty: 2,
          total: 520,
        },
      ],
    };
  },
  components: {
    Navbar,
    // Switcher,
    Footer,
    Carousel,
    Slide,
    ArrowUpIcon,
  },
  methods: {
    increase(val) {
      this.list.map((product) => {
        if (product.id === val) {
          product.qty += 1;
        }
      });
    },
    decrement(val) {
      this.list.map((product) => {
        if (product.id === val) {
          while (product.qty > 0) {
            product.qty -= 1;
          }
        }
      });
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
              <h1 class="title">Carrito</h1>
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
                      Carrito
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
          <div class="col-12">
            <div class="table-responsive bg-white shadow">
              <table class="table table-center table-padding mb-0">
                <thead>
                  <tr>
                    <th class="py-3" style="min-width: 20px"></th>
                    <th class="py-3" style="min-width: 300px">Producto</th>
                    <th class="text-center py-3" style="min-width: 160px">
                      Precio
                    </th>
                    <th class="text-center py-3" style="min-width: 160px">
                      Cantidad
                    </th>
                    <th class="text-center py-3" style="min-width: 160px">
                      Total
                    </th>
                  </tr>
                </thead>

                <tbody>
                  <tr v-for="(item, index) of list" :key="index">
                    <td class="h6">
                      <a href="javascript:void(0)" class="text-danger">X</a>
                    </td>
                    <td>
                      <div class="d-flex align-items-center">
                        <img
                          :src="item.image"
                          class="img-fluid avatar avatar-small rounded shadow"
                          style="height: auto"
                          alt=""
                        />
                        <h6 class="mb-0 ml-3">{{ item.title }}</h6>
                      </div>
                    </td>
                    <td class="text-center">$ {{ item.price }}.00</td>
                    <td class="text-center">
                      <input
                        type="button"
                        value="-"
                        class="minus btn btn-icon btn-soft-primary font-weight-bold"
                        @click="decrement(item.id)"
                      />
                      <input
                        type="text"
                        v-model="item.qty"
                        step="1"
                        min="1"
                        name="quantity"
                        value="2"
                        title="Qty"
                        class="btn btn-icon btn-soft-primary font-weight-bold ml-1"
                      />
                      <input
                        type="button"
                        value="+"
                        class="plus btn btn-icon btn-soft-primary font-weight-bold ml-1"
                        @click="increase(item.id)"
                      />
                    </td>
                    <td class="text-center font-weight-bold">
                      ${{ item.total }}.00
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>
          </div>
          <!--end col-->
        </div>
        <!--end row-->
        <div class="row">
          <div class="col-lg-8 col-md-6 mt-4 pt-2">
            <a href="javascript:void(0)" class="btn btn-primary"
              >Seguir Comprando</a
            >
            <a href="javascript:void(0)" class="btn btn-soft-primary ml-2"
              >Vaciar Carrito</a
            >
          </div>
          <div class="col-lg-4 col-md-6 ml-auto mt-4 pt-2">
            <div class="table-responsive bg-white rounded shadow">
              <table class="table table-center table-padding mb-0">
                <tbody>
                  <tr>
                    <td class="h6">Subtotal</td>
                    <td class="text-center font-weight-bold">$ 2190</td>
                  </tr>
                  <tr>
                    <td class="h6">IVA</td>
                    <td class="text-center font-weight-bold">$ 219</td>
                  </tr>
                  <tr class="bg-light">
                    <td class="h6">Total</td>
                    <td class="text-center font-weight-bold">$ 2409</td>
                  </tr>
                </tbody>
              </table>
            </div>
            <div class="mt-4 pt-2 text-right">
              <router-link to="/shop-checkouts" class="btn btn-primary"
                >Pagar Compra</router-link
              >
            </div>
          </div>
          <!--end col-->
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
