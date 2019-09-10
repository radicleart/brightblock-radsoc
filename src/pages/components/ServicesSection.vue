<template>
<div class="container" >
  <section class="text-center my-5">
    <h2 class="h1-responsive font-weight-bold my-5">Products and Services</h2>
    <p class="grey-text w-responsive mx-auto mb-5">Through developing real time decentralised blockchain based services
    Radicle have built up a level of expertise and a knowledge base across technologies like Bitcion, Ethereum and Blockstack
    that we wish to share to support the growth of the community and furtherment of this family of ground breaking technologies.</p>
    <div class="row" >
      <div class="col-md-12 mb-4">
        <card class="p-0 card bg-dark text-white border-0" style="background-image: url(https://mdbootstrap.com/img/Photos/Others/img%20%2832%29.jpg)">
          <div slot="header" class="text-white text-center rgba-black-strong py-5 px-4 rounded">
            <h6 class="text-primary">
              <i class="fas fa-certificate"></i><strong> Provenance</strong>
            </h6>
            <h3 class="py-3 font-weight-bold">
              <strong>Proof of Ownership</strong>
            </h3>
          </div>
          <template slot="raw-content">
            <div class="text-white text-center d-flex align-items-center rgba-black-strong py-5 px-4 rounded">
              <div>
                <p class="pb-3"><strong>Radicle are building tools which enable registration of both physical and digital assets on-chain creating proofs of ownership and generation of certificates of authenticity secured by the most secure blockchain available!</strong></p>
                <a class="btn btn-primary btn-md" target="_blank" href="https://medium.com/@radiclesociety/radicle-peer-to-peer-marketplaces-whats-the-deal-767960da195b"><i class="fas fa-external-link-alt"></i> Read more</a>
              </div>
            </div>
          </template>
        </card>
      </div>
      <div class="col-md-6 md-0 mb-4">
        <card class="p-0 card bg-dark text-white border-0" style="background-image: url(https://mdbootstrap.com/img/Photos/Others/img%20%2832%29.jpg)">
          <div slot="header" class="text-white text-center rgba-black-strong py-5 px-4 rounded">
            <h6 class="text-primary lighten-4">
              <i class="fab fa-bitcoin"></i><strong> Digital Rights</strong>
            </h6>
            <h3 class="py-3 font-weight-bold">
              <strong>Payment Splitting</strong>
            </h3>
          </div>
          <template slot="raw-content">
            <div class="text-white text-center d-flex align-items-center rgba-black-strong py-5 px-4 rounded">
              <div>
                <p class="pb-3"><strong>On-chain payments allow copyright and digital rights of artists, authors, creators in general to be respected on secondary and subsequent sales of their work!</strong></p>
                <a class="btn btn-primary btn-md" target="_blank" href="https://medium.com/@radiclesociety/problems-of-decentralised-applications-f6176381c75a"><i class="fas fa-external-link-alt"></i> Read more</a>
              </div>
            </div>
          </template>
        </card>
      </div>
      <div class="col-md-6 md-0 mb-4">
        <card class="p-0 card bg-dark text-white border-0" style="background-image: url(https://mdbootstrap.com/img/Photos/Others/img%20%2832%29.jpg)">
          <div slot="header" class="text-white text-center rgba-black-strong py-5 px-4 rounded">
            <h6 class="text-primary">
              <i class="fas fa-gavel"></i><strong> Auctions</strong>
            </h6>
            <h3 class="py-3 font-weight-bold">
              <strong>Transparent and Secure Bidding</strong>
            </h3>
          </div>
          <template slot="raw-content">
            <div class="text-white text-center d-flex align-items-center rgba-black-strong py-5 px-4 rounded">
              <div>
                <p class="pb-3"><strong>Auction software - backed by smart contracts - that brings security and transparency to end users and protects them from fraudulent practices!</strong></p>
                <a class="btn btn-primary btn-md" target="_blank" href="https://medium.com/@radiclesociety/user-owned-data-and-web-3-0-60c51ec11764"><i class="fas fa-external-link-alt"></i> Read more</a>
              </div>
            </div>
          </template>
        </card>
      </div>
    </div>
  </section>
</div>
</template>
<script>
import { Card, Tabs, TabPane } from '@/components';

export default {
  name: 'Services',
  components: {
    Card,
    Tabs,
    TabPane,
  }
};
</script>
<style>
</style>
