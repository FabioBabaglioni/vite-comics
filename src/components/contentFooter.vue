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
                    text: "DC POWER VISA",
                },

            ]
        }
    }
}
</script>

<template>
    <footer>

        <div id="container_small">
            <!-- sezione info sito -->
            <section class="container_card">
                <div class="card" v-for="(card, index) in cards" :key="index">
                    <img class="small_img" :src="card.img" alt="">
                    <span class="text">{{ card.text }}</span>
                </div>
            </section>

            <!-- sezione navigazione sito completa e logo  -->
            <section>
                <div class="sfondo">

                </div>
            </section>

            <!-- sezione sign up -->
            <section>

            </section>
        </div>

    </footer>
</template>

<style scoped lang="scss">
@use "./styles/partials/variables" as *;

footer {
    background-color: $brandPrimaryColor;
}

#container_small {
    width: 65%;
    margin: 0 auto;
}

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
</style>