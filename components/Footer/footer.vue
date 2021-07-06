<template>
  <div class="footer">
    <v-container-fluid>
      <v-row align-content="center" data-aos="fade-up" data-aos-delay="200">
        <v-col cols="12" sm="3">
          <div class="footer__title">Products.</div>
          <div class="footer__content">
            <span>ChartFX Studio</span>
            <span> ChartFX for Visual Studio | .Net</span>
            <span> ChartFX for HTML5 | JS</span>
            <span> ChartFX for COM | ASP </span>
            <span> ChartFX for JAVA </span>
            <span>ChartFX Cloud - Soon</span>
          </div>
        </v-col>
        <v-col cols="12" sm="3">
          <div class="footer__title">Charts.</div>
          <div class="footer__content">
            <span>Gallery</span>
            <span> Industries</span>
            <span>Use Cases</span>
            <span>Free Trials</span>
          </div>
        </v-col>
        <v-col cols="12" sm="3">
          <div class="footer__title">Resources.</div>
          <div class="footer__content">
            <span>News</span>
            <span>Documentation</span>
            <span>APIs</span>
            <span>Pricing </span>
            <span> Licensing </span>
            <span>Support</span>
          </div>
        </v-col>
        <v-col cols="12" sm="3">
          <div class="footer__title">Company.</div>
          <div class="footer__content">
            <span>About</span>
            <span>Partners</span>
            <span> Become an affiliate</span>
            <span> Terms of use </span>
            <span> Privacy policy </span>
          </div>
        </v-col>
      </v-row>
    </v-container-fluid>
    <div class="footer__copyright" data-aos="fade-up" data-aos-delay="200">
      <div class="footer__logo">
        <img :src="require('@/assets/images/chartfx-dark-logo-jop.svg')" />
      </div>
      <div class="footer__social">
        <span>
          <img
            src="https://uploads-ssl.webflow.com/5beab1239ac88487c3a6608f/5db8171e6c50c2ea0da89a03_webflow_w.svg"
          />
        </span>
        <span>
          <img
            src="https://uploads-ssl.webflow.com/5beab1239ac88487c3a6608f/5db44b53c3881181e4439bec_twit_fv.svg"
          />
        </span>
        <span>
          <img
            src="https://uploads-ssl.webflow.com/5beab1239ac88487c3a6608f/5db44b9556a86140c5ac547d_insta.svg"
          />
        </span>
        <span>
          <img
            src="https://uploads-ssl.webflow.com/5beab1239ac88487c3a6608f/5db82c473233bcbb730dacec_Discord-Logo-Color%20(2).svg"
          />
        </span>
      </div>
      <div class="footer__rights">
        <v-icon color="#0a1f44">mdi-alpha-c-circle-outline</v-icon> 2021
        ChartFX. All rights reserved.
      </div>
    </div>
  </div>
</template>

<script>
import aosMixin from '~/mixins/aos'

export default {
  name: 'Footer',
  mixins: [aosMixin],
  data() {
    return {}
  },
}
</script>

<style lang="scss" src="./footer.scss" />