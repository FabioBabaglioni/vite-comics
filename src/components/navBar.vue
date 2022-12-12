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

    <header class="">
        <img src="../../public/img/dc-logo.png" alt="">

        <ul>
            <li v-for="(link, index) in links" :key="index">
                <a href="{{link.url}}">{{ link.text }}</a>
            </li>
        </ul>
    </header>



</template>

<style scoped>
header {
    height: 80px;
    display: flex;
    justify-content: space-around;
    padding: 12px 0;
}

a {
    text-decoration: none;
    color: black;
    font-size: 15px;
}

a:hover {
    color: #0c7cec;
    padding-bottom: 40px;
    border-bottom: 5px solid #0c7cec;

}

ul {
    display: flex;
    justify-content: space-between;
}

li {
    list-style-type: none;
    padding: 10px;
}
</style>