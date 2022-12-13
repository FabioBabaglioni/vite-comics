<script>

export default {
    data() {
        return {
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

            <img id="logo" src="../../public/img/dc-logo-bg.png" alt="">




        </div>
    </section>
</template>

<style scoped lang="scss">
@use "./styles/partials/variables" as *;

#sfondo {
    padding: 20px 0;
    background-image: url("../../public/img/footer-bg.jpg");
    background-size: cover;
    height: 400px;
    overflow: hidden;


    .container_flex {
        display: flex;
        justify-content: flex-start;

        .container_ul {
            margin-right: 50px;

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

        #logo {
            margin-top: -20px;
        }
    }



}
</style>