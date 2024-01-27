<script setup lang="ts">

</script>

<template>
  <header class="header">
    <div class="container">
      <div class="header-left">
        <div class="logo">
          <a href="#" title="FOSACHA">
            <img src="https://fosacha.com/upload/config/original/fosacha-1645000405.png" alt="">
          </a>
        </div>
      </div>

      <div class="header-right">
        <div class="menu">
          <div class="menu-hamburger">
            <div class="menu-hamburger-line"></div>
            <div class="menu-hamburger-line"></div>
            <div class="menu-hamburger-line"></div>
          </div>
          <div class="menu-close d-lg-none">
            <a href="javascript:;" class="jsClose-mobileMenu">
              <img src="https://fosacha.com/template/images/ic-close-menu.svg" alt="">
            </a>
          </div>

          <div class="menu-items">
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
                <a href="#" activelink="" link="" class="nav__link
                                       ">
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

            <ul class="list-contact-menu my-4 my-lg-5 d-flex d-lg-none">
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

            <ul class="list-social-menu d-flex d-lg-none">
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
.header {
  position: fixed;
  top: 50px;
  left: 0;
  right: 0;
  z-index: 111;
  margin: 0 15px;
  //transition: ;
}

.container {
  position: relative;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  background: #181818;
  border-radius: 60px;
  padding: 20px 40px;
}

.logo {
  width: 180px;
  height: 40px;
}

.header-right {
  position: relative;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  margin-left: auto;
}

.menu {
  display: block;
}

.list-contact-menu {
  position: relative;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 10px;
}

.list-social-menu {
  position: relative;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  gap: 30px;
}

.d-flex {
  display: flex !important;
}

.my-4 {
  margin-top: 1.5rem !important;
  margin-bottom: 1.5rem !important;
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

  .my-lg-5 {
    margin-top: 3rem !important;
    margin-bottom: 3rem !important;
  }

  .menu-sub {
    position: absolute;
    opacity: 0;
    visibility: hidden;
    transform: translate(0, 20px);
    transition: all .3s;
  }

  .header .menu-links:hover::before, .header .menu-links.active::before {
    width: 80px;
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