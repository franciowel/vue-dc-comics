<template>
    <div class="color">
        <div class="contain flexcontain">
            <ContentCards v-for="element, index in comics" :key="index" :comicDetails="element" />
        </div>
        <div class="flex">
            <a class="btn" href="#">
                LOAD MORE
            </a>
        </div>
    </div>
</template>

<script>
import ComicJson from '../assets/dc-comics.json';
import ContentCards from './ContentCards.vue';
export default {
    name: "ContentComponent",
    components: { 
        ContentCards
        },
    data() {
        return {
            comics: ComicJson
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/color.scss';
@import '../style/font.scss';

.color{
    background-color: #1c1c1c;
    color: white;
    padding: 3rem 0;
    .contain{
        height: 100%;
        align-items: center;
        flex-wrap: wrap;
        span{
            font-size: 1.5rem;
            font-family: Arial, Helvetica, sans-serif;
        }
    }
    .flex{
        display: flex;
        justify-content: center;
        
    }
    .btn{
        background-color: $primary;
        font-family: $similfont;
        padding: 0.8rem 5rem;
        color: white;
        font-weight: 600;
        margin-top: 1rem;
    }
}
</style>