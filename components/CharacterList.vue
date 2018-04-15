<template>
    <v-card>
        <v-toolbar color="secondary" dark>
            <v-toolbar-title>Characters</v-toolbar-title>
            <v-spacer></v-spacer>
        </v-toolbar>
        <v-list>
            <character-list-item
            v-for="character in characters"
            v-bind:key="character.name"
            v-bind:character="character"
            ></character-list-item>
        </v-list>
    </v-card>
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
