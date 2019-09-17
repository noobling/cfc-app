<template>
  <v-app>
    <v-app-bar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>Vuetify</span>
        <span class="font-weight-light">
          <v-btn to="/">MATERIAL DESIGN</v-btn>
        </span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn @click="goAbout">
        <span class="mr-2">Latest Release</span>
      </v-btn>
    </v-app-bar>

    <v-content>
      <HelloWorld />
    </v-content>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue';
import HelloWorld from './components/HelloWorld.vue';

export default Vue.extend({
  name: 'App',
  components: {
    HelloWorld,
  },
  data: () => ({
    //
  }),
  methods: {
    goAbout() {
      this.$router.push('/about')
    }
  },
});
</script>
