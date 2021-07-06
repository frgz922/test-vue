<template>
  <div class="hero">
    <div class="hero__text-container">
      <div class="hero__title" data-aos="fade-left">
        {{ heroTitle }}
      </div>
      <div class="hero__subtitle" data-aos="fade-left" data-aos-delay="100">
        {{ heroSubtitle }}
      </div>
      <div class="hero__buttons" data-aos="fade-left" data-aos-delay="150">
        <v-btn depressed color="#000" width="48%" height="50px">
          Download a free trial
        </v-btn>
        <v-btn depressed color="primary" width="48%" height="50px">
          Buy ChartFX for Visual Studio
          <v-icon right color="white"> mdi-arrow-right </v-icon>
        </v-btn>
      </div>
      <div class="hero__footer" data-aos="fade-left" data-aos-delay="200">
        <img :src="require('@/assets/images/visual-studio-icon-content.svg')" />
        <div>{{ heroFooter }}</div>
      </div>
    </div>
    <div class="hero__background"></div>
  </div>
</template>

<script>
import aosMixin from '~/mixins/aos'

export default {
  name: 'Hero',
  mixins: [aosMixin],
  data() {
    return {
      heroTitle:
        'The most advanced features in a single product for Visual Studio',
      heroSubtitle:
        'Chart FX for Visual Studio is the most powerful and versatile multi-platform tool for Web and Desktop Data Visualization in the industry.',
      heroFooter:
        'AVAILABLE FOR VISUAL STUDIO 2010, 2012, 2013, 2015, 2017, 2019.',
    }
  },
}
</script>

<style lang="scss" src="./hero.scss" />