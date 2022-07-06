<template>
<div class="color">
    <div class="contain flexcontain">
        <div class="services" v-for="element in ServiceBanner" :key="element">
            <img v-bind:src="element.img" :alt="element.text">
            <p>{{ element.text }}</p>
        </div>
    </div>
</div>
    
</template>

<script>
export default {
    name: 'ServiceBanner',
    data() {
        return {
            serviceContent: [
                {
                    img: require('../assets/img/buy-comics-digital-comics.png'),
                    text: 'DIGITAL COMICS'
                },
                {
                    img: require('../assets/img/buy-comics-shop-locator.png'),
                    text: 'DC MERCHANDISE'
                },
                {
                    img: require('../assets/img/buy-comics-merchandise.png'),
                    text: 'SUBSCRIPTION'
                },
                {
                    img: require('../assets/img/buy-comics-subscriptions.png'),
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    img: require('../assets/img/buy-dc-power-visa.svg'),
                    text: 'DC POWER VISA'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/color.scss';
@import '../style/commons.scss';
.color{
    background-color: $primary;
    height: 180px;
}
.services {
    display: flex;
    align-items: center;
    img {
        width: 78px;
        padding: 10px;
    }
}
.flexcontain{
        align-items: center;
        height: 100%;
        color: white;
        justify-content: space-evenly;
    }
div {
    img {
        width: 50%;
    }
}

</style>