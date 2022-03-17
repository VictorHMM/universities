<template>
  <v-container>
    <ul>
      <li v-for="uni in unisArray" :key="uni.name">{{ uni.name }}</li>
    </ul>
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
