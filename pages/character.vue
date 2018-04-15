<template>
<div>
    <character-list v-bind:characters="characters"/>
</div>
</template>


<script>
import CharacterList from '~/components/CharacterList.vue'

export default {
  components: {
    CharacterList
  },
  data: function () {
    return {
      title: 'Characters',
      characters: [
        { id: 1, name: 'Atlas' },
        { id: 2, name: 'Skip Jarret' }
      ]
    }
  }
}
</script>
