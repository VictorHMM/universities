<template>
    <v-container>
        <h2 class="text-h5 text-center mb-3 mt-5">Universities</h2>
        <UnisList :universities="unisArray"/>
    </v-container>
</template>

<script>
import UnisList from '../components/shared/UnisList.vue';
export default {
    name: 'UnisListView',
    components: {
        UnisList,
    },
    data: () => {
        return {
            unisArray: []
        }
    },
    created() {
        fetch('http://universities.hipolabs.com/search?country=United+Kingdom')
            .then(response => response.json())
            .then((json) => {this.unisArray = json})
            console.log(this.unisArray)
    }
}
</script>

<style scoped>

</style>