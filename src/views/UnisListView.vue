<template>
    <v-container>
        <h2 class="text-h5 text-center mb-3 mt-5"> Universities</h2>
        <UnisList/>
    </v-container>
</template>

<script>
import UnisList from "../components/shared/UnisList.vue";
export default {
    data: () => {
        return {
            unisList: []
        }
    }
}
</script>

<style scoped>

</style>