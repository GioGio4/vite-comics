<script>
export default {

    props: {
        ComicInfo: Object,
    },
}
</script>

<template>
    <div class="card">
        <img :src="ComicInfo.thumb" alt="comic">
        <h3>{{ ComicInfo.series }}</h3>
        <p>{{ ComicInfo.price }}</p>
        <p>{{ ComicInfo.type }}</p>
    </div>
</template>

<style lang="scss"  scoped>
.card {
    width: calc(15% - 40px);
    margin: 0 20px;




}
</style>