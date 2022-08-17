<template>
  <v-app>
    <v-main>
      <HomeLanding />
    </v-main>
  </v-app>
</template>

<script>
import HomeLanding from './components/HomeLanding.vue';

export default {
  name: 'App',
  components: {
    HomeLanding
  },
  data: () => ({})
};
</script>
