<template>
  <v-app>
    <AppTopBar/>
      <v-main>
        <UnisList/>
    </v-main>
  </v-app>
</template>

<script>
import AppTopBar from './components/shared/AppTopBar.vue'
import UnisList from './components/shared/UnisList.vue'

export default {
  name: 'App',

  components: {
    AppTopBar,
    UnisList,
  },

  data: () => ({
    //
  }),
};
</script>
