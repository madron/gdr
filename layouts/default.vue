<template>
  <v-app>
    <v-tabs color="primary" show-arrows>
      <v-tabs-slider color="black"></v-tabs-slider>
      <v-tab :to="item.to" :key="i" v-for="(item, i) in items" nuxt replace>{{ item.title }}</v-tab>
    </v-tabs>
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          { icon: 'home', title: 'Home', to: '/' },
          { icon: 'people', title: 'Characters', to: '/character' }
        ]
      }
    }
  }
</script>
