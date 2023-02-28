<script>
import Card from './Card.vue';

export default {

    props: {
        ComicsList: Array,
    },

    components: { Card },
};

</script>

<template>
    <section>

        <div class="card-container">
            <Card v-for="comic in ComicsList" :ComicInfo="comic" />

        </div>
    </section>
</template>

<style lang="scss" scoped>
/* Debug */

section {

    background-color: #1c1c1c;
    color: white;
    padding: 100px 200px;


    .card-container {
        max-width: 1400px;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
    }

}
</style>