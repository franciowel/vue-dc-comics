<template>
    <section class="background">
        <div class="contain">
            <div class="flexcontain">
                <div>
                    <div class="foot-link-col">
                        <span class="title-foot">DC COMICS</span>
                        <ul>
                            <li v-for="link in dcComics" :key="link">
                                <a href="#">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>

                    <div class="foot-link-col">
                        <span class="title-foot">SHOP</span>
                        <ul>
                            <li v-for="link in shop" :key="link">
                                <a href="#">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>

                <div>
                    <div class="foot-link-col">
                        <span class="title-foot">DC</span>
                        <ul>
                            <li v-for="link in dc" :key="link">
                                <a href="#">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>

                <div>
                    <div class="foot-link-col">
                        <span class="title-foot">SITES</span>
                        <ul>
                            <li v-for="link in sites" :key="link">
                                <a href="#">{{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>

                <div>
                    <img class="logo" src="../assets/img/dc-logo-bg.png" alt="logo">
                </div>

            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'FooterLink',
    data() {
        return {
            dcComics: [
                {
                    text: 'Characters',
                    active: false
                },
                {
                    text: 'Comics',
                    active: false
                },
                {
                    text: 'Movies',
                    active: false
                }, 
                {
                    text: 'TV',
                    active: false
                },
                {
                    text: 'Games',
                    active: false
                },
                {
                    text: 'Videos',
                    active: false
                },
                {
                    text: 'News',
                    active: false
                }
            ],
            shop: [
                {
                    text: 'Shop DC',
                    active: false
                }, 
                {
                    text: 'Shop DC Collectibles',
                    active: false
                }
            ],
            dc: [
                {
                    text: 'Terms Of Use',
                    active: false
                }, 
                {
                    text: 'Privacy Policy (New)',
                    active: false
                },
                {
                    text: 'Ad Choices',
                    active: false
                },
                {
                    text: 'Adversiting',
                    active: false
                },
                {
                    text: 'Jobs',
                    active: false
                },
                {
                    text: 'Subscriptions',
                    active: false
                },
                {
                    text: 'Talent Workshop',
                    active: false
                },
                {
                    text: 'CPSC Certificates',
                    active: false
                },
                {
                    text: 'Ratings',
                    active: false
                },
                {
                    text: 'Shop Help',
                    active: false
                },
                {
                    text: 'Contact Us',
                    active: false
                }
            ],
            sites: [
                {
                    text: 'DC',
                    active: false
                },
                {
                    text: 'MAD Magazine',
                    active: false
                },
                {
                    text: 'DC Kids',
                    active: false
                },
                {
                    text: 'DC Universe',
                    active: false
                },
                {
                    text: 'DC Power Visa',
                    active: false
                },
            ]
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
    .logo {
        width: 60%;
        overflow: hidden;
    }
}
</style>