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
                        <ul class="list-top-footer">
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>Tv</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <h3>shop</h3>
                        <ul class="list-top-footer">
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                    <div class="col-2">
                        <h3>dc</h3>
                        <ul class="list-top-footer">
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
                        <ul class="list-top-footer">
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                    <div class="col-6">
                        <img class="img-dc" src="/dc-logo-bg.png" alt="">
                    </div>
                </div>
            </div>

        </div>
        <div class="bottom-footer">
            <div class="container">
                <div class="row">
                    <div class="col-6">
                        <button class="color-button">sign-up now!</button>
                    </div>
                    <div class="col-6 d-flex align-items-center justify-content-end ">
                        <span>follow us</span>
                        <ul class="list-bottom-footer">
                            <li><img src="/public/footer-facebook.png" alt=""></li>
                            <li><img src="/public/footer-youtube.png" alt=""></li>
                            <li><img src="/public/footer-twitter.png" alt=""></li>
                            <li><img src="/public/footer-pinterest.png" alt=""></li>
                            <li><img src="/public/footer-periscope.png" alt=""></li>
                            
                        </ul>
                    </div>
                </div>
            </div>
        </div>  
        
    </footer>
</template>
<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.top-footer {
    background-image: url(/footer-bg.jpg);
    position: relative;

}

h3 {
    text-transform: uppercase;
    color: $colore-secondario;
    padding-top: 20px;
}

h3:hover {
    color: $colore-primario;
}

.list-top-footer {
    padding: 0px;

    li {
        color: rgb(156, 154, 154);
        list-style: none;
        padding: 5px 0px;
    }

    li:hover {
        color: $colore-secondario;
        cursor: pointer;
    }
}

.img-dc {
    position: relative;
    bottom: 50px;
}

.bottom-footer {
    background-color: rgba(48, 48, 48, 255);
    position: absolute;
    top: 970px;
    width: 100%;
}

.color-button {
    text-transform: uppercase;
    color: $colore-secondario;
    background-color: transparent;
    border: 2px solid $colore-primario;
    padding: 5px 10px;
    margin: 30px 0px;

    &:hover {
        background-color: $colore-primario;
    }

}

.list-bottom-footer {

    display: flex;
    list-style: none;
    vertical-align: middle;
    margin: 0;




    li {
        padding: 0px 10px;


    }

}

span {
    color: $colore-primario;
    text-transform: uppercase;
    font-size: 24px;
    font-weight: 600;
    vertical-align: middle;
}
</style>