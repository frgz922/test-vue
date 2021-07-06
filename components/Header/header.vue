<template>
  <div class="header">
    <div class="header__logo">
      <img :src="require('@/assets/images/chartfx-lite-logo-jop.svg')" alt="" />
    </div>
    <div class="header__items">
      <span>
        Products
        <v-icon right dark> mdi-chevron-down </v-icon>
      </span>
      <span>
        Charts
        <v-icon right dark> mdi-chevron-down </v-icon>
      </span>
      <span>
        Pricing
        <v-icon right dark> mdi-chevron-down </v-icon>
      </span>
      <span>
        Resources
        <v-icon right dark> mdi-chevron-down </v-icon>
      </span>
      <span>
        Company
        <v-icon right dark> mdi-chevron-down </v-icon>
      </span>
    </div>
    <div>
      <v-btn color="primary" depressed>Login</v-btn>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style lang="scss" src="./header.scss" />