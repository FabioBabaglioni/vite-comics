<script>
import jumbotron from './jumbotron.vue'

export default {
    components: {
        jumbotron
    },
    props: {
        card: Array
    }
}
</script>

<template>
    <jumbotron />
    <main>
        <section class="container">
            <div class="container_flex">
                <div class="card" v-for="(cards, index) in card" :key="index">
                    <div class="box">
                        <img class="img_small" :src="cards.thumb" alt="">
                    </div>
                    <div class="text_series">{{ cards.series }}</div>
                </div>
            </div>

        </section>
    </main>
</template>

<style scoped lang="scss">
@use "./styles/partials/variables" as *;

main {
    background-color: #1c1c1c;

    .container_flex {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        width: 100%;

        .card {
            width: calc((100% / 6) - 10px);
            height: auto;
            padding: 20px 5px;
        }

        .box {
            width: 140px;
            height: 140px;
            overflow: hidden;
        }

        .text_series {
            color: $brandSecondaryColor;
            font-size: 15px;
            padding-top: 20px;
        }
    }




}
</style>