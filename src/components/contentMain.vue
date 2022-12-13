<script>

export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <main>
        <section class="container">
            <div class="container_flex">
                <div class="card" v-for="(card, index) in cards" :key="index">
                    <div class="box">
                        <img class="img_small"
                            src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
                            alt="">
                    </div>
                    <div class="text_series">{{ card.series }}</div>
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