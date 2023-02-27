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
    <header>
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

<style scoped>
/* Debug */

header {
    padding: 10px 200px;
}

nav {
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
