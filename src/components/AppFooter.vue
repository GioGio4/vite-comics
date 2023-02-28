<script>
export default {
    data() {
        return {
            // Footer link Data
            ComicsLink: {
                title: "DC COMICS",
                linkList: [
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
            },

            ShopLink: {
                title: "SHOP",
                linkList: [
                    {
                        title: "Shop DC",
                        link: "#",
                    },
                    {
                        title: "Shop DC Collectibles",
                        link: "#",
                    }
                ]
            },

            DcLink: {
                title: "DC",
                linkList: [
                    {
                        title: "Terms of Use",
                        link: "#"
                    },
                    {
                        title: "Privacy Policy",
                        link: "#"
                    },
                    {
                        title: "Ad Choice",
                        link: "#"
                    },
                    {
                        title: "Advertising",
                        link: "#"
                    },
                    {
                        title: "Jobs",
                        link: "#"
                    },
                    {
                        title: "Subscription",
                        link: "#"
                    },
                    {
                        title: "Talent Workshop",
                        link: "#"
                    },
                    {
                        title: "CPSC Certificates",
                        link: "#"
                    },
                    {
                        title: "Rating",
                        link: "#"
                    },
                    {
                        title: "Shop Help",
                        link: "#"
                    },
                    {
                        title: "Contact Us",
                        link: "#"
                    },
                ]
            },

            SitesLink: {
                title: "SITES",
                linkList: [
                    {
                        title: "DC",
                        link: "#"
                    },
                    {
                        title: "Mad Magazine",
                        link: "#"
                    },
                    {
                        title: "DC Kids",
                        link: "#"
                    },
                    {
                        title: "DC Universe",
                        link: "#"
                    },
                    {
                        title: "DC Power Visa",
                        link: "#"
                    },
                ]
            }
        }
    }
}
</script>

<template>
    <footer>
        <!-- List link -->
        <section class="link-container container">

            <div class="link-list">

                <div>
                    <h3>{{ ComicsLink.title }}</h3>
                    <ul>
                        <li v-for="textLink in ComicsLink.linkList">
                            <a :href="textLink.link">{{ textLink.title }}</a>
                        </li>
                    </ul>

                    <h3>{{ ShopLink.title }}</h3>
                    <ul>
                        <li v-for="textLink in ShopLink.linkList">
                            <a :href="textLink.link">{{ textLink.title }}</a>
                        </li>
                    </ul>
                </div>

                <div>
                    <h3>{{ DcLink.title }}</h3>
                    <ul>
                        <li v-for="textLink in DcLink.linkList">
                            <a :href="textLink.link">{{ textLink.title }}</a>
                        </li>
                    </ul>
                </div>

                <div>
                    <h3>{{ SitesLink.title }}</h3>
                    <ul>
                        <li v-for="textLink in SitesLink.linkList">
                            <a :href="textLink.link">{{ textLink.title }}</a>
                        </li>
                    </ul>
                </div>

            </div>
            <div class="logo-container">
            </div>
        </section>

        <section class="social">
            <div class="container d-flex">
                <div>

                    <button class="btn-sign" type="button">SIGN-UP NOW</button>
                </div>

                <!-- Aggiungere link social (adesso solo img) -->
                <div class="social-link">
                    <h3>FOLLOW US</h3>
                    <img src="../assets/img/footer-facebook.png" alt="facebook">
                    <img src="../assets/img/footer-twitter.png" alt="twitter">
                    <img src="../assets/img/footer-youtube.png" alt="youtube">
                    <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                    <img src="../assets/img/footer-periscope.png" alt="periscope">

                </div>

            </div>
        </section>

    </footer>
</template>

<style lang="scss" scoped>
/* Debug */
footer {
    max-height: 100%;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;

}

.link-container {
    display: flex;
    justify-content: space-between;
    padding: 20px 0;
}

.social {
    background-color: rgb(49, 49, 49);
    padding: 20px 0;
}

.link-list {
    display: flex;
}

.link-list>div {
    margin: 0 1rem;
}


h3 {
    color: white;
    margin: .5rem 0;
}

.logo-container {
    width: 30%;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-size: contain;
    background-repeat: no-repeat;
}

a {
    color: grey;
    font-size: 12px;
}

.d-flex {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.social-link {
    display: flex;
    justify-content: space-between;

    h3 {
        color: #0282f9;
    }
}

.social-link>img {
    width: 2rem;
    height: 2rem;
    margin: 0 .5rem;
}

.btn-sign {
    color: white;
    background-color: transparent;
    border: 2px solid #0282f9;
    padding: .7rem 1.3rem;
}
</style>