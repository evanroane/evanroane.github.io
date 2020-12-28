<template>
  <div>
    <TopNavigation />
    <Nuxt />
    <Footer />
  </div>
</template>

<script lang="ts">
import Footer from '~/components/Footer.vue';
import TopNavigation from '~/components/TopNavigation.vue';

export default {
  components: { Footer, TopNavigation }
}
</script>
