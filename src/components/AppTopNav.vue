<template>
    <v-app-bar>
        <template #prepend>
            <v-icon icon="mdi-bookmark-multiple-outline"></v-icon>
        </template>

        <v-app-bar-title>Vue Bookmarks</v-app-bar-title>

        <template #append>
            <v-btn>Login</v-btn>
        </template>

        <template #extension>
            <CategoryTabs />
        </template>
    </v-app-bar>
</template>

<script setup>
</script>
