<script>
export default {

    props: {
        ComicInfo: Object,
    },
}
</script>

<template>
    <div class="card">
        <div class="image">
            <img :src="ComicInfo.thumb" alt="comic">
        </div>
        <div class="text-area">
            <h4>{{ ComicInfo.series }}</h4>
            <p>{{ ComicInfo.price }}</p>
            <p>{{ ComicInfo.type }}</p>
        </div>
    </div>
</template>

<style lang="scss"  scoped>
.card {
    display: flex;
    flex-direction: column;
    width: calc(15% - 30px);
    height: 250px;
    margin: 10px 15px;


    .image {
        height: 70%;

        img {
            height: 100%;
            width: 100%;
            object-fit: cover;
            object-position: top;
        }
    }

    .text-area {
        margin-top: .5rem;
    }





}
</style>