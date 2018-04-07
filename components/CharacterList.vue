<template>
  <div class="CharacterList">
    <ul>
        <character-list-item
        v-for="character in characters"
        v-bind:key="character.name"
        v-bind:character="character"
        ></character-list-item>
    </ul>
  </div>
</template>

<script>
import CharacterListItem from './CharacterListItem.vue'

export default {
    components: {
        CharacterListItem
    },
    props: {
        characters: {
            type: Array,
            default: function() {
                return []
            },
        },
    },
}
</script>
