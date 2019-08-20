<template>
  <div>
    <div class="page-header clear-filter" filter-color="blue">
      <parallax
        class="page-header-image"
        style="background-image:url('img/header.jpg')"
      >
      </parallax>
      <div class="container">
        <div class="content-center brand">
          <h1 class="h1-seo">Web 3.0 Auctions and Peer to Peer Marketplaces</h1>
          <h3>Blockchain technology changes the rules of the game!</h3>
        </div>
      </div>
    </div>
    <services-section/>
    <blockstack-dapps-section></blockstack-dapps-section>
    <consultancy-section/>
    <reference-apps-section></reference-apps-section>
    <download-section></download-section>
  </div>
</template>
<script>
import { Parallax } from '@/components';
import ServicesSection from './components/ServicesSection';
import BlockstackDappsSection from './components/BlockstackDappsSection';
import ReferenceAppsSection from './components/ReferenceAppsSection';
import DownloadSection from './components/DownloadSection';
import ConsultancySection from './components/ConsultancySection';

export default {
  name: 'index',
  bodyClass: 'index-page',
  components: {
    Parallax,
    ServicesSection,
    BlockstackDappsSection,
    ConsultancySection,
    ReferenceAppsSection,
    DownloadSection
  }
};
</script>
<style>
.rgba-black-strong, .rgba-black-strong:after {
    background-color: rgba(0,0,0,.7);
}
.card.card-image {
    background-size: cover;
    background-position: center;
    width: 100%;
}
.btn-rounded {
    border-radius: 10em;
}
.btn-secondary {
    background-color: #a6c!important;
    color: #fff;
}
</style>
