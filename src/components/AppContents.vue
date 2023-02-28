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

        <div class="container">

            <div class="card-container">
                <Card v-for="comic in ComicsList" :ComicInfo="comic" />
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
/* Debug */

section {

    background-color: #1c1c1c;
    color: white;
    padding: 50px 0;


    .card-container {
        display: flex;
        flex-wrap: wrap;
    }

}
</style>