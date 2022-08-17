<template>
  <v-app>
    <v-main>
      <HomeLanding />
      <FooterBlock />
    </v-main>
  </v-app>
</template>

<script>
import HomeLanding from './components/HomeLanding.vue';
import FooterBlock from './components/FooterBlock.vue';

export default {
  name: 'App',
  components: {
    HomeLanding,
    FooterBlock
  },
  data: () => ({})
};
</script>
