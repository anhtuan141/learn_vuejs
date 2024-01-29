<script setup lang="ts">

</script>

<template>
  <header class="header bg-gray-900 fixed top-10 left-0 right-0 z-50 mx-4 rounded-full">
    <div class="container flex items-center justify-between py-5 px-10 bg-gray-900 rounded-full">
      <div class="header-left">
        <div class="logo">
          <a href="#" title="FOSACHA">
            <img class="inline" src="https://fosacha.com/upload/config/original/fosacha-1645000405.png" alt="">
          </a>
        </div>
      </div>

      <div class="header-right flex items-center">
        <div class="menu">
          <div class="menu-hamburger flex flex-col justify-between cursor-pointer lg:hidden">
            <div class="menu-hamburger-line h-1 w-6 bg-white mb-1"></div>
            <div class="menu-hamburger-line h-1 w-6 bg-white mb-1"></div>
            <div class="menu-hamburger-line h-1 w-6 bg-white"></div>
          </div>
          <div class="menu-close d-lg-none lg:block">
            <a href="javascript:;">
              <img src="https://fosacha.com/template/images/ic-close-menu.svg" alt="">
            </a>
          </div>

          <div class="menu-items hidden lg:flex flex-col lg:flex-row lg:items-center lg:justify-between">
            <div class="menu-links active">
              <div class="menu-parent">
                <a href="#" activelink="" link="https://fosacha.com/introduce"
                   class="nav__link">
                  About
                </a>
              </div>
            </div>
            <div class="menu-links">
              <div class="menu-parent">
                <a href="#" activelink="" link="https://fosacha.com/product"
                   class="nav__link">
                  Product
                </a>
                <i class="fa fa-chevron-down" aria-hidden="true"></i>
              </div>
              <div class="menu-sub">
                <div class="menu-sub-items">
                  <a href="#" title="E-Brochures" class="">E-Brochures</a>
                </div>
              </div>
            </div>
            <div class="menu-links">
              <div class="menu-parent">
                <a href="#" activelink="" link="" class="nav__link">
                  News
                </a>
                <i class="fa fa-chevron-down" aria-hidden="true"></i>
              </div>
              <div class="menu-sub">
                <div class="menu-sub-items">
                  <a href="#" title="CORPORATE NEWS" class="">CORPORATE NEWS</a>
                  <a href="#" title="BLOG" class="">BLOG</a>
                  <a href="#" title="CAREERS" class="active">CAREERS</a>
                </div>
              </div>
            </div>
            <div class="menu-links">
              <div class="menu-parent">
                <a href="#" activelink="" link="" class="nav__link">
                  Contact
                </a>
                <i class="fa fa-chevron-down" aria-hidden="true"></i>
              </div>
              <div class="menu-sub">
                <div class="menu-sub-items">
                  <a href="#" title="Contact info" class="">Contact info</a>
                  <a href="#" title="Registration form" class="">Registration form</a>
                </div>
              </div>
            </div>

            <ul class="list-contact-menu my-6 lg:my-12 flex d-lg-none">
              <li>
                <a href="mail:info@fosacha.com">
                  <img src="https://fosacha.com/template/images/ic-contact-menu-1.svg" alt="">
                  <span>info@fosacha.com</span>
                </a>
              </li>

              <li>
                <a href="(+84)866 090 366">
                  <img src="https://fosacha.com/template/images/ic-contact-menu-2.svg" alt="">
                  <span>(+84)866 090 366</span>
                </a>
              </li>
            </ul>

            <ul class="list-social-menu d-lg-none relative flex flex-wrap items-center justify-center gap-8">
              <li>
                <a href="https://www.youtube.com/channel/UCm0rzF-RIM9vUY6eUFg8J_w">
                  <img src="https://fosacha.com/template/images/ic-social-menu-1.svg" alt="">
                </a>
              </li>

              <li>
                <a href="https://www.linkedin.com/company/fosachajsc/">
                  <img src="https://fosacha.com/template/images/ic-social-menu-2.svg" alt="">
                </a>
              </li>

              <li>
                <a href="https://wa.me/84866090366">
                  <img src="https://fosacha.com/template/images/ic-social-menu-3.svg" alt="">
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
.logo {
  width: 180px;
  height: 40px;
}

.menu {
  display: block;
}

.header .menu-parent {
  position: relative;
  z-index: 1;
}

.header .menu-links:not(:last-child) {
  margin-right: 70px;
}

@media (max-width: 991px) {
  .menu .menu-hamburger-line {
    height: 2px;
    background: #333;
    margin: 4px auto 4px 0;
    width: 18px
  }

  .menu .menu-hamburger.menu-open {
    display: none
  }
}

@media (min-width: 992px) {
  .menu-items {
    display: flex;
    flex-flow: row;
    align-items: center;
    justify-content: space-between;
  }

  .menu-links {
    position: relative;
  }

  .d-lg-none {
    display: none !important;
  }

  .menu-sub {
    position: absolute;
    opacity: 0;
    visibility: hidden;
    transform: translate(0, 20px);
    transition: all .3s;
  }

  .header .menu-links:hover::before,
  .header .menu-links.active::before {
    @apply w-20;
  }

  .header .menu-links::before {
    content: "";
    position: absolute;
    background: #129d49;
    width: 0;
    height: 2px;
    left: 50%;
    bottom: -10px;
    transform: translateX(-50%);
    transition: all .3s;
  }
}
</style>