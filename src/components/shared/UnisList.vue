<template>
  <v-container>
<v-simple-table>
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
        <tr
          v-for="uni in unisArray"
          :key="uni.name"
        >
          <td>{{ uni.name }}</td>
          <td>{{ uni.webPages[0] }}</td>
        </tr>
      </tbody>
    </template>
  </v-simple-table>
  </v-container>
</template>

<script>
export default {
  name: "UnisList",
  data: () => {
    return {
      unisArray: [
        {
          name: "Futureworks",
          country: "United Kingdom",
          webPages: ["https://futureworks.ac.uk/"],
        },
        {
          name: "University of Arts of London",
          country: "United Kingdom",
          webPages: ["https://arts.ac.uk/"],
        },
        {
          name: "University of Aberdeen",
          country: "United Kingdom",
          webPages: ["https://abdn.ac.uk/"],
        },
      ],
    };
  },
};
</script>

<style scoped></style>
