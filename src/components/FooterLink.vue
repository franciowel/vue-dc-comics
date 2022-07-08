<template>
    <section class="background">
        <div class="contain">
            <div class="flexcontain">
                
                <div class="col-contain">

                    <div>
                        <div class="foot-link-col">
                            <span class="title-foot">DC COMICS</span>
                            <ul>
                                <li v-for="item, index in dcComics" :key="index">
                                    <a href="#">{{item.text}}</a>
                                </li>
                            </ul>
                        </div>

                        <div class="foot-link-col">
                            <span class="title-foot">SHOP</span>
                            <ul>
                                <li v-for="item, index in shop" :key="index">
                                    <a href="#">{{item.text}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>

                    <div>
                        <div class="foot-link-col">
                            <span class="title-foot">DC</span>
                            <ul>
                                <li v-for="item, index in dc" :key="index">
                                    <a href="#">{{item.text}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>

                    <div>
                        <div class="foot-link-col">
                            <span class="title-foot">SITES</span>
                            <ul>
                                <li v-for="item, index in sites" :key="index">
                                    <a href="#">{{item.text}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>

                </div>

            </div>

            <div class="flex">
                <img class="logo" src="../assets/img/dc-logo-bg.png" alt="logo">
            </div>

        </div>
    </section>
</template>

<script>
import TextData from '../assets/dc-comics-link.json';
import ShopLink from '../assets/shop-link.json';
import DcLinks from '../assets/dc-links.json';
import SitesLink from '../assets/sites-link.json';

export default {
    name: 'FooterLink',
    data() {
        return {
            dcComics: TextData,
            shop: ShopLink,
            dc: DcLinks,
            sites: SitesLink,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/commons.scss';
@import '../style/color.scss';
@import '../style/font.scss';

.background{
    background-image: url('../assets/img/footer-bg.jpg');
    color: white;
    height: 450px;
    overflow: hidden;
    position: relative;
}
.title-foot{
    color: white;
    font-weight: 600;
}

li {
    color: grey;
    padding: 0.2rem 0;
}

.foot-link-col{
    padding: 2rem 1rem;
}

.contain{
    font-family: $similfont;
    justify-content: space-between;
    display: flex;
    .col-contain{
        display: flex;
        width: 40%;
        margin-right: 2rem;
    }
    .flex{
        display: flex;
        justify-content: center;
        align-content: center;
    }
    .logo {
        width: 90%;
        transform: scale(1.2);
    }
}
</style>