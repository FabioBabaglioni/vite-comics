<script>

export default {
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    active: "true"
                },
                {
                    text: "COMICS",
                    url: "#",
                    active: "false"
                },
                {
                    text: "MOVIES",
                    url: "#",
                    active: "false"
                },
                {
                    text: "TV",
                    url: "#",
                    active: "false"
                },
                {
                    text: "GAMES",
                    url: "#",
                    active: "false"
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    active: "false"
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    active: "false"
                },
                {
                    text: "FANS",
                    url: "#",
                    active: "false"
                },
                {
                    text: "NEWS",
                    url: "#",
                    active: "false"
                },
                {
                    text: "SHOP",
                    url: "#",
                    active: "false"
                },
            ]
        }
    }
}
</script>

<template>

    <header class="container">
        <img src="../../public/img/dc-logo.png" alt="">

        <ul>
            <li v-for="(link, index) in links" :key="index">
                <a href="{{link.url}}">{{ link.text }}</a>
            </li>
        </ul>
    </header>



</template>

<style scoped lang="scss">
@use "./styles/partials/variables" as *;

header {
    height: 100px;

}

ul {
    display: flex;
    justify-content: space-between;
    align-items: center;

    li {
        list-style-type: none;
        padding: 10px;
    }

    a {
        text-decoration: none;
        color: black;
        font-size: 15px;

        &:hover {
            color: $brandPrimaryColor;
            padding-bottom: 29px;
            border-bottom: 5px solid $brandPrimaryColor;

        }
    }
}
</style>