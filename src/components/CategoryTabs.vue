<template>
    <v-tabs 
        v-model="tab" 
        align-tabs="title"
        :items="tabItems"
        center-active
        show-arrows
    >
        <template v-slot:tab="{ item }">
            <v-tab
                :text="item.text"
                :value="item.value"
                class="text-none"
            >
                <template v-if="item.icon" #prepend>
                    <v-icon :icon="item.icon"></v-icon>
                </template>
            </v-tab>
        </template>
    </v-tabs>
</template>

<script setup>
import { ref } from 'vue'

let tab = ref(null)
let tabItems = ref([
    {
        icon: 'mdi-lock-outline',
        value: 'me',
        text: 'Me',
    },
    {
        value: 'applications',
        text: 'Applications',
    },
    ,
    {
        value: 'other',
        text: 'Other',
    },
    ,
    {
        value: 'utility',
        text: 'Utility',
    },
    {
        value: 'wikis',
        text: 'Wikis',
    }
])
</script>
