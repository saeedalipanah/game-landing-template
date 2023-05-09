<template>
  <div class="home">
    <!-- header-area -->
    <Header></Header>
    <!-- header-area-end -->

    <!-- main-area -->
    <main>
      <!-- slider-area -->
     <SiteBanner></SiteBanner>

      <!-- information-area -->
      <Information></Information>

      <!-- game-gallery-area -->
      <GameGalery></GameGalery>

      <!-- my-match-area -->
      <Matches></Matches>

      <!-- donation-area -->
      <Donation></Donation>

      <!-- team-area -->
      <Teams></Teams>

      <!-- contact-area -->
      <ContactUs></ContactUs>

      <!-- brand-area -->
      <Brands></Brands>
    </main>
    <!-- main-area-end -->

    <!-- footer-area -->
    <Footer></Footer>
  </div>
</template>

<script>
import Header from "@/components/containers/Header.vue";
import SiteBanner from "@/components/home/SiteBanner.vue";
import Information from "@/components/home/Information.vue";
import GameGalery from "@/components/home/GameGalery.vue";
import Matches from "@/components/home/Matches.vue";
import Donation from "@/components/home/Donation.vue";
import Teams from "@/components/home/Teams.vue";
import ContactUs from "@/components/home/ContactUs.vue";
import Brands from "@/components/home/Brands.vue";
import Footer from "@/components/containers/Footer.vue";
export default {
  data() {
    return {};
  },
  components: {
    Header,
    SiteBanner,
    Information,
    GameGalery,
    Matches,
    Donation,
    Teams,
    ContactUs,
    Brands,
    Footer,
  },
};
</script>
