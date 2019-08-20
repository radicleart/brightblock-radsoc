<template>
<mdb-container>
  <section class="text-center">
    <h2 class="h1-responsive font-weight-bold my-5">Blockchain Consultancy</h2>
    <p class="grey-text w-responsive mx-auto mb-5">Radicle Society are a group of technologists and blockchain enthusiasts based in Brighton, UK
    united by the shared desire to help realise the transformative possibilities of this technology for everyone.</p>
    <mdb-row>
      <mdb-col md="12" class="mb-4">
        <mdb-card class="card-image" style="background-image: url(img/header.jpg)">
          <div class="text-white text-center d-flex align-items-center rgba-black-strong py-5 px-4 rounded">
            <div>
              <h6 class="text-primary">
                <i class="far fa-question-circle"></i><strong> Questions?</strong>
              </h6>
              <h3 class="py-3 font-weight-bold">
                <strong>We can help!</strong>
              </h3>
              <p class="pb-3"><strong>If you want to understand more about the benefits of decentralised technology - self owned online identity
              and user controlled data...</strong></p>
              <a class="btn btn-primary btn-md" target="_blank" href="mailto:mijoco@radiclesociety.org?subject=Info radicle Society">Send Us an Email</a>
            </div>
          </div>
        </mdb-card>
      </mdb-col>
    </mdb-row>
  </section>
</mdb-container>
</template>
<script>
import { Card, Tabs, TabPane } from '@/components';
import { mdbContainer, mdbRow, mdbCol, mdbView, mdbMask, mdbCard, mdbCardBody, mdbBtn, mdbIcon } from 'mdbvue';

export default {
  name: 'Services',
  components: {
    Card,
    Tabs,
    TabPane,
    mdbContainer,
    mdbRow,
    mdbCol,
    mdbView,
    mdbMask,
    mdbCard,
    mdbCardBody,
    mdbBtn,
    mdbIcon
  }
};
</script>
<style>
.tab-content.tab-content-padding {
  padding: 20px;
}

</style>
