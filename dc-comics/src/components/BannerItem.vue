<script>
export default {
    name:'BannerItem',
    data() {
        return{
            cards: [
                {
                    img: '/img/buy-comics-digital-comics.png',
                    title: 'Digital comics'
                },
                {
                    img: '/img/buy-comics-merchandise.png',
                    title: 'DC Merchandise'
                },
                {
                    img: '/img/buy-comics-shop-locator.png',
                    title: 'Comic Shop Locator'
                },
                {
                    img: '/img/buy-comics-subscriptions.png',
                    title: 'Subscriptions'
                },
                {
                    img: '/img/buy-dc-power-visa.svg',
                    title: 'Dc Power Visa'
                }
            ]
        }
    }


}
</script>

<template>

    <div class="features">
        <div class="container">

            <div class="card" v-for="card in cards">
                <div>
                    <img :src="`${card.img}`" alt="feature_img">
                    <span>{{ card.title }}</span>
                </div>
            </div>
        </div>
    </div>



</template>