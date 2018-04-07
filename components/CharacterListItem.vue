<template>
  <div>
    <v-card>
      <v-card-title primary-title><h3>{{ character.name }}</h3></v-card-title>
    </v-card>
  </div>
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
