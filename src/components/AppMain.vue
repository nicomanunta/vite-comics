<script>
export default {
    name: "AppMain",
    data() {
        return {
            links: [
                {
                    img: "buy-comics-digital-comics.png",
                    label: "DIGITAL COMICS",
                    url: "#"
                },
                {
                    img: "buy-comics-merchandise.png",
                    label: "DC MERCHANDISE",
                    url: "#"
                },
                {
                    img: "buy-comics-subscriptions.png",
                    label: "SUBSCRIPTIONS",
                    url: "#"
                },
                {
                    img: "buy-comics-shop-locator.png",
                    label: "COMIC SHOP LOCATOR",
                    url: "#"
                },
                {
                    img: "buy-dc-power-visa.svg",
                    label: "DC POWER VISA",
                    url: "#"
                },
            ]
        }
    },
}
</script>
<template lang="">
    <main>
        <div class="films">
            <div class="container">
                <div class="row">
                    <div class="col-12">
                        <h1 class="titolo">-->Content goes here<--</h1>
                    </div>
                </div>
            </div>
        </div>
        <div class="dc-info">
            <div class="container">
                <div class="row">
                    <div class="col-12">
                        <ul>
                            <li v-for="link, index in links" :key="index">
                                <span><img class="immagini" :src="link.img" alt=""></span>
                                <span>{{link.label}}</span>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>
<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.films {
    background-color: black;
}

.titolo {
    color: $colore-secondario;
    padding: 50px 0px;
}

ul {
    display: flex;
    justify-content: center;
    list-style: none;
    height: 100%;
    align-items: center;

    li span {
        padding: 10px;
        text-decoration: none;
        color: $colore-secondario;

    }

}

.immagini {
    width: 50px;
}

.dc-info {
    background-color: $colore-primario;
    padding: 50px 0px;
}
</style>