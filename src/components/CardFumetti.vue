<script>
export default {
    name: "CardFumetti",
    props: {
        fumetto: Array
    }
}
</script>
<template lang="">
    <div class="col-2 d-flex mt-4" >
        <div style="width: 18rem;">
            <img class="img-fumetti" :src="fumetto.thumb" alt="">
            <div class="distanza">
                <h6> {{fumetto.series}} </h6>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.img-fumetti {
    width: 100%;
    height: 200px;
}

h6 {
    color: $colore-secondario;
}

.distanza {
    margin-top: 10px
}
</style>