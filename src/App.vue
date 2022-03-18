<template>
  <v-app>
    <AppTopBar/>
      <v-main>
        <UnisListView/>
    </v-main>
  </v-app>
</template>

<script>
import AppTopBar from './components/shared/AppTopBar.vue'
import UnisListView from './views/UnisListView.vue'

export default {
  name: 'App',

  components: {
    AppTopBar,
    UnisListView,
  },

  data: () => ({
    //
  }),
};
</script>
