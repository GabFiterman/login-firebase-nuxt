<template>
  <v-app dark>
    <Breadcrumbs />
    <Nuxt />
  </v-app>
</template>

<script>
import Breadcrumbs from '~/components/Breadcrumbs.vue';
export default {
    name: "DefaultLayout",
    components: { Breadcrumbs }
}
</script>

