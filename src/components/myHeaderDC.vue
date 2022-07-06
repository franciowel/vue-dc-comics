<template>
    <div class="contain">
        <div class="flexcontain">

            <div class="logohead">
                <img src="../assets/img/dc-logo.png" alt="Logo Dc" class="logo">
            </div>

            <div class="navbar">
                
                <ul class="flexcontain">
                    <li v-for="link in navbarLink" :key="link" :class="{'active' : link.active}">
                        <span :class="{'color': link.active}">{{link.text}}</span>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'myHeaderDc',
    data () {
        return {
            navbarLink: [
                {
                    text: 'CHARACTERS',
                    active: false
                },
                {
                    text: 'COMICS',
                    active: true
                },
                {
                    text: 'MOVIES',
                    active: false
                },
                {
                    text: 'TV',
                    active: false
                },
                {
                    text: 'GAMES',
                    active: false
                },
                {
                    text: 'COLLECTIBLES',
                    active: false
                },
                {
                    text: 'VIDEOS',
                    active: false
                },
                {
                    text: 'FANS',
                    active: false
                },
                {
                    text: 'NEWS',
                    active: false
                },
                {
                    text: 'SHOP',
                    active: false
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import url('../style/commons.scss');
@import url('../style/color.scss');
.logohead{
    width: 25%;
}
.navbar{
    width: 60%;
}
.logo {
    width: 25%;
    padding-top: 1.3rem;
}
li {
    padding: 5px;
    font-weight: 500;
    align-self: center;
    font-size: 0.9rem;
    &.active {
        border-bottom: solid #2481f4 3px;
    }
    
}
.color{
    color: #2481f4;
}
ul {
    height: 100%;
    line-height: 82px;
}

.contain {
    font-family: Arial, Helvetica, sans-serif;
    .flexcontain {
        justify-content: space-between;
    }
}
</style>