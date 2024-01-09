<script>
export default {
    name: "AppFooter",
    data() {
        return {

        }
    },
}
</script>
<template lang="">
    <footer>
        <div class="top-footer">
            <div class="container">
                <div class="row">
                    <div class="col-2">
                        <h3>dc comics</h3>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>Tv</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <h3>shop</h3>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>

                        </ul>
                    </div>
                    <div class="col-2">
                        <h3>dc</h3>
                        <ul>
                            <li>Terms Of Use</li>
                            <li>Privacy Police (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Helps</li>
                            <li>Contact Us</li>

                        </ul>
                    </div>
                    <div class="col-2">
                        <h3>sites</h3>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>

                        </ul>
                    </div>
                    <div class="col-6">

                    </div>
                </div>
            </div>

        </div>
        <div class="bottom-footer">
  
        </div>  
        
    </footer>
</template>
<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.top-footer {
    background-image: url(/footer-bg.jpg);

}

h3 {
    text-transform: uppercase;
    color: $colore-secondario;
    padding-top: 20px;
}

h3:hover {
    color: $colore-primario;
}

ul {
    padding: 0px;

    li {
        color: rgb(156, 154, 154);
        list-style: none;
        padding: 5px 0px;
    }

    li:hover {
        color: $colore-secondario;
    }
}
</style>