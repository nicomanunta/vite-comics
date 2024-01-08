<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    label: "CHARACTERS",
                    url: "#",
                    current: false
                },
                {
                    label: "COMICS",
                    url: "#",
                    current: true
                },
                {
                    label: "MOVIES",
                    url: "#",
                    current: false
                },
                {
                    label: "TV",
                    url: "#",
                    current: false
                },
                {
                    label: "GAMES",
                    url: "#",
                    current: false
                },
                {
                    label: "COLLECTIBLES",
                    url: "#",
                    current: false
                },
                {
                    label: "VIDEOS",
                    url: "#",
                    current: false
                },
                {
                    label: "FANS",
                    url: "#",
                    current: false
                },
                {
                    label: "NEWS",
                    url: "#",
                    current: false
                },
                {
                    label: "SHOP",
                    url: "#",
                    current: false
                },
            ]

        }
    },
}
</script>
<template lang="">
    <header>
        <div class="container">
            <div class="row">
                <div class="col-3 ">
                    <img src="/dc-logo.png" alt="">
                </div>
                <div class="col-9">
                    <ul>
                        <li v-for="link, index in links" :key="index">
                            <a :class="link.current ? 'active' : ' ' "  :href="link.url">
                            {{link.label}}
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>
<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

header {
    margin: 20px 0px;
}



ul {
    display: flex;
    justify-content: end;
    list-style: none;
    height: 100%;
    align-items: center;

    li a {
        padding: 10px;
        text-decoration: none;


        &.active {
            color: $colore-primario;
        }
    }

}
</style>