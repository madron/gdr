<template>
  <v-list-tile>
      <v-list-tile-title>{{ character.name }}</v-list-tile-title>
  </v-list-tile>
</template>

<script>
export default {
  props: {
    character: {
      type: Object
    }
  }
}
</script>
