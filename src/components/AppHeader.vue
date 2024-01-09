<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    label: "CHARACTERS",
                    url: "#",
                    current: true
                },
                {
                    label: "COMICS",
                    url: "#",
                    current: true
                },
                {
                    label: "MOVIES",
                    url: "#",
                    current: true
                },
                {
                    label: "TV",
                    url: "#",
                    current: true
                },
                {
                    label: "GAMES",
                    url: "#",
                    current: true
                },
                {
                    label: "COLLECTIBLES",
                    url: "#",
                    current: true
                },
                {
                    label: "VIDEOS",
                    url: "#",
                    current: true
                },
                {
                    label: "FANS",
                    url: "#",
                    current: true
                },
                {
                    label: "NEWS",
                    url: "#",
                    current: true
                },
                {
                    label: "SHOP",
                    url: "#",
                    current: true
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
                <div class="col-9 d-flex align-items-center justify-content-end  ">
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

    list-style: none;



    li a {
        padding: 10px;
        padding-bottom: 50px;
        text-decoration: none;



        &.active:hover {
            color: $colore-primario;
            border-bottom: 4px solid $colore-primario;
        }
    }

}
</style>