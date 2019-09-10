<template>
<div class="container" >
  <section class="text-center">
    <h2 class="h1-responsive font-weight-bold my-5">Blockchain Consultancy</h2>
    <p class="grey-text w-responsive mx-auto mb-5">Radicle Society are a group of technologists and blockchain enthusiasts based in Brighton, UK
    united by the shared desire to help realise the transformative possibilities of this technology for everyone.</p>
    <div class="row">
      <div class="col-12">
        <card class="p-0 card bg-dark text-white border-0" style="background-image: url(img/header.jpg)">
          <div slot="header" class="text-white text-center rgba-black-strong py-5 px-4 rounded">
            <h6 class="text-primary"><i class="far fa-question-circle"></i><strong> Questions?</strong></h6>
            <h3 class="py-1 font-weight-bold">
              <strong>We can help!</strong>
            </h3>
          </div>
          <div slot="raw-content" class="text-white text-center d-flex align-items-center rgba-black-strong py-1 px-4 rounded">
            <div>
              <p class="pb-1"><strong>If you want to understand more about the benefits of decentralised technology - self owned online identity
              and user controlled data...</strong></p>
              <a class="btn btn-primary btn-md" target="_blank" href="mailto:mijoco@radiclesociety.org?subject=Info radicle Society">Send Us an Email</a>
            </div>
          </div>
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
