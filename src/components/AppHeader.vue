<script>
export default {
    data() {
        return {
            NavLogo: "dc-logo.png",

            NavList: [
                {
                    title: "Characters",
                    link: "#"
                },
                {
                    title: "Comics",
                    link: "#"
                },
                {
                    title: "Movies",
                    link: "#"
                },
                {
                    title: "Tv",
                    link: "#"
                },
                {
                    title: "Games",
                    link: "#"
                },
                {
                    title: "Collectibles",
                    link: "#"
                },
                {
                    title: "Video",
                    link: "#"
                },
                {
                    title: "Fans",
                    link: "#"
                },
                {
                    title: "News",
                    link: "#"
                },
                {
                    title: "Shop",
                    link: "#"
                },

            ]
        };
    },
};

</script>

<template>
    <header class="container">
        <nav>
            <!-- Logo -->
            <!-- logo gestito come Path relativo, ma andrà usato come Path dinamico -->
            <img src="../assets/img/dc-logo.png" alt="logo">
            <!-- List Link -->
            <ul>
                <li v-for="navlink in NavList">
                    <a :href="navlink.link">{{ navlink.title }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<!-- Gestire lo style con SASS -->
<style scoped>
/* Debug */


nav {
    margin: 10px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

img {
    width: 70px;
}

li {
    display: inline-block;
    margin: 0 .5rem;
}
</style>
