<template>
<mdb-navbar expand="medium" color="blue-grey lighten-1" light>
  <mdb-navbar-brand>
    <router-link to="/" class="nav-link navbar-link"><img :src="logo" width="90px" alt="main logo"></router-link>
  </mdb-navbar-brand>
  <mdb-navbar-toggler>
    <mdb-navbar-nav center class="">
        <router-link class="nav-link navbar-link text-nowrap btn btn-sm teal lighten-1 px-3 text-white" style="max-width: 100px; font-weight: 600;" to="/buy">BUY <i class="fas fa-angle-down text-dark ml-2 fa-1x"></i></router-link>
        <router-link class="nav-link navbar-link text-nowrap btn btn-sm deep-orange lighten-1 px-3 text-white" style="max-width: 100px; font-weight: 600;" to="/sell">SELL <i class="fas fa-angle-up text-dark mr-auto fa-1x"></i></router-link>
    </mdb-navbar-nav>
    <div class="d-md-none d-sm-block">
      <mdb-navbar-nav right class="">
        <account-links-xs/>
      </mdb-navbar-nav>
    </div>
    <div class="d-none d-md-block">
      <mdb-navbar-nav right class="" style="width: 120px;">
        <account-links v-if="loggedIn"/>
      </mdb-navbar-nav>
    </div>
    <mdb-navbar-nav tag="li" v-if="!loggedIn"  style="min-width: 100px;">
      <a v-on:click.prevent="loginMultiPlayer" class="nav-link navbar-link">Login <i class="fas fa-sign-in-alt"></i></a>
    </mdb-navbar-nav>
  </mdb-navbar-toggler>
</mdb-navbar>
</template>

<script>
import { DropDown, NavbarToggleButton, Navbar, NavLink } from '@/components';
import { Popover } from 'element-ui';
import myAccountService from "brightblock-lib/src/services/myAccountService";
import { mdbContainer, mdbNavbar, mdbNavbarBrand, mdbNavbarToggler, mdbNavbarNav, mdbNavItem, mdbDropdown, mdbDropdownMenu, mdbDropdownToggle, mdbInput, mdbDropdownItem } from 'mdbvue';
export default {
  name: 'main-navbar',
  props: {
    transparent: Boolean,
    colorOnScroll: Number
  },
  components: {
    DropDown,
    Navbar,
    NavbarToggleButton,
    NavLink,
    [Popover.name]: Popover,
    mdbContainer, mdbNavbar, mdbNavbarBrand, mdbNavbarToggler, mdbNavbarNav, mdbNavItem, mdbDropdown, mdbDropdownMenu, mdbDropdownToggle, mdbInput, mdbDropdownItem
  },
  computed: {
    showDownload() {
      const excludedRoutes = ["login", "landing", "profile"];
      return excludedRoutes.every(r => r !== this.$route.name);
    },
    showAdmin() {
      return this.$store.state.myAccountStore.myProfile.showAdmin;
    },
    username() {
      return this.$store.state.myAccountStore.myProfile.name;
    },
    avatar() {
      let myProfile = this.$store.getters["myAccountStore/getMyProfile"];
      if (myProfile.loggedIn) {
        return (
          '<img style="width: 40px; height: 40px; border-radius: 20px;" src="' +
          myProfile.avatarUrl +
          '"/>'
        );
      } else {
        return '<i class="fas fa-user"></i>';
      }
    },
    loggedIn() {
      let myProfile = this.$store.getters["myAccountStore/getMyProfile"];
      return myProfile.loggedIn;
    }
  },
};
</script>

<style scoped></style>
