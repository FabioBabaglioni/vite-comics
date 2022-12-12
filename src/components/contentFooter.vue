<script>

export default {
    data() {
        return {
            cards: [
                {
                    img: "../../public/img/buy-comics-digital-comics.png",
                    text: "DIGITAL COMICS",
                },
                {
                    img: "../../public/img/buy-comics-merchandise.png",
                    text: "DC MERCHANDISE",
                },
                {
                    img: "../../public/img/buy-comics-subscriptions.png",
                    text: "SUBSCRIPTION",
                },
                {
                    img: "../../public/img/buy-comics-shop-locator.png",
                    text: "COMIC SHOP LOCATOR",
                },
                {
                    img: "../../public/img/buy-dc-power-visa.svg",
                    text: "DC POWER VISA"
                },
            ],

            dcComics:
                [
                    {
                        text: "Characters",
                        url: "#"
                    },
                    {
                        text: "Comics",
                        url: "#"
                    },
                    {
                        text: "Movies",
                        url: "#"
                    },
                    {
                        text: "Tv",
                        url: "#"
                    },
                    {
                        text: "Games",
                        url: "#"
                    },
                    {
                        text: "Videos",
                        url: "#"
                    },
                    {
                        text: "news",
                        url: "#"
                    },

                ],

            shop: [

                {
                    text: "Shop DC",
                    url: "#"
                },
                {
                    text: "Shop DC collection",
                    url: "#"
                }
            ],

            dc:
                [
                    {
                        text: "Term of use",
                        url: "#"
                    },
                    {
                        text: "Privacy police (new)",
                        url: "#"
                    },
                    {
                        text: "Ad Choices",
                        url: "#"
                    },
                    {
                        text: "Advertising",
                        url: "#"
                    },
                    {
                        text: "Jobs",
                        url: "#"
                    },
                    {
                        text: "Subscriptions",
                        url: "#"
                    },
                    {
                        text: "Talent Workshop",
                        url: "#"
                    },
                    {
                        text: "CPSC Certificates",
                        url: "#"
                    },
                    {
                        text: "Ratings",
                        url: "#"
                    },
                    {
                        text: "Shop Help",
                        url: "#"
                    },
                    {
                        text: "Contact Us",
                        url: "#"
                    },

                ],

            sites:
                [
                    {
                        text: "DC",
                        url: "#"
                    },
                    {
                        text: "MAD Magazine",
                        url: "#"
                    },
                    {
                        text: "DC Kids",
                        url: "#"
                    },
                    {
                        text: "DC Universal",
                        url: "#"
                    },
                    {
                        text: "DC Power Visa",
                        url: "#"
                    },

                ],
        }
    }
}
</script>

<template>
    <footer>
        <!-- sezione info sito -->
        <section id="bg_color_brand">
            <div id="container_small" class="container_card">
                <div class="card" v-for="(card, index) in cards" :key="index">
                    <img class="small_img" :src="card.img" alt="">
                    <span class="text">{{ card.text }}</span>
                </div>
            </div>
        </section>

        <!-- sezione navigazione sito completa e logo  -->
        <section id="sfondo">
            <div class="container">

                <div class="container_flex">
                    <div class="container_ul">
                        <h2>DC COMICS</h2>
                        <ul class="pb_2">
                            <li v-for="(link, index) in dcComics" :key="index">
                                {{ link.text }}
                            </li>
                        </ul>

                        <h2>SHOP</h2>
                        <ul>
                            <li v-for="(link, index) in shop" :key="index">
                                {{ link.text }}
                            </li>
                        </ul>
                    </div>

                    <div class="container_ul">
                        <h2>DC</h2>
                        <ul>
                            <li v-for="(link, index) in dc" :key="index">
                                {{ link.text }}
                            </li>
                        </ul>
                    </div>

                    <div class="container_ul">
                        <h2>SITES</h2>
                        <ul>
                            <li v-for="(link, index) in sites" :key="index">
                                {{ link.text }}
                            </li>
                        </ul>
                    </div>
                </div>

                <div id="logo_footer">

                </div>

            </div>
        </section>

        <!-- sezione sign up -->
        <section>

        </section>


    </footer>
</template>

<style scoped lang="scss">
@use "./styles/partials/variables" as *;


#container_small {
    width: 65%;
    margin: 0 auto;
}

#bg_color_brand {
    background-color: $brandPrimaryColor;

    .container_card {
        padding: 20px 0;
        display: flex;
        justify-content: space-between;
    }

    .card {
        display: flex;
        align-items: center;
        color: white;
    }

    .small_img {
        max-width: 35px;
        margin-right: 10px;
    }
}

#sfondo {
    padding: 20px 0;
    background-image: url("../../public/img/footer-bg.jpg");
    background-size: cover;
    height: 400px;


    .container_flex {
        display: flex;
        justify-content: flex-start;

        .container_ul {
            margin-right: 70px;

            .pb_2 {
                padding-bottom: 20px;
            }

            h2 {
                font-size: 20px;
                color: white;

                &:hover {
                    color: $brandPrimaryColor;
                    cursor: pointer;
                }

            }

            li {
                color: lightgrey;
                margin: 10px 0;
                font-size: 12px;

                &:hover {
                    color: $brandPrimaryColor;
                    cursor: pointer;
                }
            }
        }

    }



}
</style>