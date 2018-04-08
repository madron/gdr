<template>
  <v-app>

    <v-tabs color="primary" show-arrows>
      <v-tabs-slider color="black"></v-tabs-slider>
      <v-tab to="/" nuxt replace>Home</v-tab>
      <v-tab to="/character" nuxt replace>Characters</v-tab>
    </v-tabs>

    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>

    <!-- <v-navigation-drawer :clipped="clipped" :floating="floating" v-model="drawer" fixed app>
      <v-list>
        <v-list-tile router :to="item.to" :key="i" v-for="(item, i) in items" exact>
          <v-list-tile-action>
            <v-icon v-html="item.icon"></v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title v-text="item.title"></v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer> -->


  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        clipped: true,
        drawer: false,
        floating: true,
        items: [
          { icon: 'home', title: 'Home', to: '/' },
          { icon: 'info', title: 'About', to: 'about' },
          { icon: 'people', title: 'Characters', to: 'character' }
        ],
        title: '',
        tab: null,
        items: [
          'web', 'shopping', 'videos', 'images', 'news'
        ],
        text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'      }
    }
  }
</script>
