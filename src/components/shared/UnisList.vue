<template>
  <v-container>
<v-simple-table class="width-100%">
    <template v-slot:default>
      <thead>
        <tr>
          <th class="text-left">
            Name
          </th>
          <th class="text-left">
            Webpage
          </th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="uni in universities" :key="uni.name">
          <td>{{ uni.name }}</td>
          <td>{{ uni.web_pages[0] }}</td>
        </tr>
      </tbody>
    </template>
  </v-simple-table>
  </v-container>
</template>

<script>
export default {
  name: 'UnisList',
  props: {
    universities: {
        type: Array,
        required: true
    }
  }
};
</script>

<style scoped></style>
