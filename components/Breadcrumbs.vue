<template>
    <div id="Breadcrumbs">
        <v-breadcrumbs :items="items">
            <template v-slot:divider>
                <v-icon>mdi-chevron-right</v-icon>
            </template>
        </v-breadcrumbs>
    </div>
</template>

<script>
export default {
name: "Breadcrumbs"
}
</script>

<style scoped>
#Breadcrumbs{
    background-color: lightslategray;
    min-height: 5rem;
}
</style>