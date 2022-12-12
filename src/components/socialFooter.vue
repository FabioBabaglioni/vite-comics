<script>

export default {
    data() {
        return {

        }
    }
}
</script>

<template>

    <!-- sezione sign UP e social -->
    <section>

        <div class="container">
            <div id="btn">SIGN-UP NOW</div>

            <div class="container_flex">
                <div class="text_color pr-15">FOLLOW US</div>
                <img class="pr-15" src="../../public/img/footer-facebook.png" alt="">
                <img class="pr-15" src="../../public/img/footer-periscope.png" alt="">
                <img class="pr-15" src="../../public/img/footer-pinterest.png" alt="">
                <img class="pr-15" src="../../public/img/footer-twitter.png" alt="">
                <img class="pr-15" src="../../public/img/footer-youtube.png" alt="">
            </div>
        </div>

    </section>
</template>

<style scoped lang="scss">
@use "./styles/partials/variables" as *;

section {
    background-color: #303030;


    #btn {
        color: white;
        border: 2px solid $brandPrimaryColor;
        padding: 10px;

        &:hover {
            border: 2px solid white;
            color: $brandPrimaryColor;
            cursor: pointer;
        }
    }

    .container_flex {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .text_color {
            color: $brandPrimaryColor;
            font-size: 18px;

            &:hover {
                color: white;
                cursor: pointer;
            }
        }

        .pr-15 {
            padding-right: 15px;
        }
    }


}
</style>