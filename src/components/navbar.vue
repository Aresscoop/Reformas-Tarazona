<script>
/**
 * Navbar component
 */
export default {
  data() {
    return {
      isCondensed: false,
    };
  },
  props: {
    isWhiteNavbar: {
      type: Boolean,
    },
    navLight: {
      type: Boolean,
    },
    isIcons: {
      type: Boolean,
    },
  },

  mounted: () => {
    window.onscroll = function () {
      onwindowScroll();
    };

    function onwindowScroll() {
      if (
        document.body.scrollTop > 50 ||
        document.documentElement.scrollTop > 50
      ) {
        document.getElementById("topnav").classList.add("nav-sticky");
      } else {
        document.getElementById("topnav").classList.remove("nav-sticky");
      }

      if (
        document.body.scrollTop > 100 ||
        document.documentElement.scrollTop > 100
      ) {
        document.getElementById("back-to-top").style.display = "inline";
      } else {
        document.getElementById("back-to-top").style.display = "none";
      }
    }

    var links = document.getElementsByClassName("side-nav-link-ref");
    var matchingMenuItem = null;
    for (var i = 0; i < links.length; i++) {
      if (window.location.pathname === links[i].pathname) {
        matchingMenuItem = links[i];
        break;
      }
    }

    if (matchingMenuItem) {
      matchingMenuItem.classList.add("active");
      var parent = matchingMenuItem.parentElement;

      /**
       * TODO: This is hard coded way of expading/activating parent menu dropdown and working till level 3.
       * We should come up with non hard coded approach
       */
      if (parent) {
        parent.classList.add("active");
        const parent2 = parent.parentElement;
        if (parent2) {
          parent2.classList.add("active");
          const parent3 = parent2.parentElement;
          if (parent3) {
            parent3.classList.add("active");
            const parent4 = parent3.parentElement;
            if (parent4) {
              const parent5 = parent4.parentElement;
              parent5.classList.add("active");
            }
          }
        }
      }
    }
  },
  methods: {
    /**
     * Toggle menu
     */
    toggleMenu() {
      this.isCondensed = !this.isCondensed;
      if (this.isCondensed) {
        document.getElementById("navigation").style.display = "block";
      } else document.getElementById("navigation").style.display = "none";
    },

    /**
     * Menu clicked show the submenu
     */
    onMenuClick(event) {
      event.preventDefault();
      const nextEl = event.target.nextSibling.nextSibling;

      if (nextEl && !nextEl.classList.contains("open")) {
        const parentEl = event.target.parentNode;
        if (parentEl) {
          parentEl.classList.remove("open");
        }
        nextEl.classList.add("open");
      } else if (nextEl) {
        nextEl.classList.remove("open");
      }
      return false;
    },
  },
};
</script>

<template>
  <div>
    <!-- Navbar STart -->
    <header
      id="topnav"
      class="defaultscroll sticky"
      :class="{ 'bg-white': isWhiteNavbar === true }"
    >
      <div class="container">
        <!-- Logo container-->
        <div>
          <router-link class="logo" to="/" v-if="navLight !== true">
            <img
              src="../../public/images/Logo_horiz_RT.png"
              width="150px"
              height="auto"
              alt=""
            />
          </router-link>
          <router-link class="logo" to="/" v-else>
            <img
              src="../../public/images/Logo_horiz_RT.png"
              class="l-dark"
              width="150px"
              height="auto"
              alt=""
            />
            <img
              src="../../public/images/Logo_horiz_RT_blanco.png"
              class="l-light"
              width="150px"
              height="auto"
              alt=""
            />
          </router-link>
        </div>
        <!-- End Logo container-->
        <div class="menu-extras">
          <div class="menu-item">
            <!-- Mobile menu toggle-->
            <a
              class="navbar-toggle"
              @click="toggleMenu()"
              :class="{ open: isCondensed === true }"
            >
              <div class="lines">
                <span></span>
                <span></span>
                <span></span>
              </div>
            </a>
            <!-- End mobile menu toggle-->
          </div>
        </div>

        <div id="navigation">
          <!-- Navigation Menu-->
          <ul
            class="navigation-menu"
            :class="{ 'nav-light': navLight === true }"
          >
            <li>
              <router-link to="/" class="side-nav-link-ref">Inicio</router-link>
            </li>
            <li>
              <router-link to="/page-portfolio-grid" class="side-nav-link-ref"
                >Proyectos</router-link
              >
            </li>
            <li>
              <router-link to="/shop-grids" class="side-nav-link-ref"
                >Productos</router-link
              >
            </li>
            <li>
              <router-link to="/page-services" class="side-nav-link-ref"
                >Servicios</router-link
              >
            </li>
            <li>
              <router-link to="/page-portfolio-detail" class="side-nav-link-ref"
                >Contract</router-link
              >
            </li>
            <li>
              <router-link to="/page-contact-three" class="side-nav-link-ref"
                >Contacto</router-link
              >
            </li>
            <div style="padding-top: 20px; padding-left: 20px">
              <a href="#"
                ><img
                  src="../../public/images/español.png"
                  width="30px"
                  height="20px"
                  style="margin-right: 10px"
              /></a>
              <a href="#"
                ><img
                  src="../../public/images/ingles.png"
                  width="30px"
                  height="20px"
              /></a>
            </div>
          </ul>

          <!--end navigation menu-->
          <!-- <div class="buy-menu-btn d-none">
            <a
              href="https://1.envato.market/4n73n"
              target="_blank"
              class="btn btn-primary"
              >Buy Now</a
            >
          </div> -->
          <!--end login button-->
        </div>
        <!--end navigation-->
      </div>
      <!--end container-->
    </header>
    <!--end header-->
    <!-- Navbar End -->
  </div>
</template>
