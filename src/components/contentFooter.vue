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

            ]
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
                <ul>
                    <li>

                    </li>
                </ul>
                <ul>
                    <li>

                    </li>
                </ul>
                <ul>
                    <li>

                    </li>
                </ul>
                <ul>
                    <li>

                    </li>
                </ul>

                <!-- <img src="../../public/img/dc-logo-bg.png" alt=""> -->
            </div>
        </section>

        <!-- sezione sign up -->
        <section>

        </section>


    </footer>
</template>

<style scoped lang="scss">
@use "./styles/partials/variables" as *;

footer {}

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

    // DEBUG
    height: 400px;

    li {
        color: white;
    }
}
</style>