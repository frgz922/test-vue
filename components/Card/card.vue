<template>
  <div class="card">
    <v-card elevation="2" outlined light height="315" class="card__body">
      <v-img max-width="60" :src="img" class="card__img"></v-img>
      <v-card-title class="card__title">{{ title }}</v-card-title>
      <v-card-text class="card__text">
        <span>{{ text }}</span>
      </v-card-text>
      <v-card-subtitle v-if="subtitle" class="card__subtitle">
        <span>{{ subtitle }}</span>
        <v-icon right light v-if="icon"> {{ icon }} </v-icon>
      </v-card-subtitle>
    </v-card>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: ['img', 'title', 'text', 'subtitle', 'icon'],
  data() {
    return {}
  },
}
</script>

<style lang="scss" src="./card.scss" />

