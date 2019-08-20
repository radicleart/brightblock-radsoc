<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <nav>
        <ul>
          <!--
          <li><a href="https://dbid.io">Bidding</a></li>
          <li><a href="https:///radicle.art">Provenance</a></li>
          -->
          <li><a href="https://medium.com/@radiclesociety/problems-of-decentralised-applications-f6176381c75a">Blog</a></li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}, with <i class="far fa-heart"></i>&nbsp; <a href="https://radiclesociety.org">radiclesociety.org</a>.
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>
