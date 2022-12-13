<script>

export default {

}
</script>

<template>
    <section class="jumbotron">
        <h1>CURRENT SERIES</h1>
    </section>

</template>

<style scoped lang="scss">
@use "./styles/partials/variables" as *;

.jumbotron {
    background-image: url(../../public/img/jumbotron.jpg);
    background-size: cover;
    height: 300px;
    position: relative;
}


h1 {
    color: $brandSecondaryColor;
    padding: 10px;
    background-color: $brandPrimaryColor;
    font-size: 20px;
    font-weight: 600;
    position: absolute;
    left: 220px;
    bottom: -20px;
}
</style>