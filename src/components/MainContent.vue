<template>
    <div class="color">
        <div class="contain flexcontain">
            <ContentCards v-for="element, index in comics" :key="index" :comicDetails="element" />
        </div>
        <div class="flex">
            <div class="btn">
                LOAD MORE
            </div>
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
.color{
    background-color: #1c1c1c;
    color: white;
    // height: 150px;
    padding: 1rem 0;
    .contain{
        height: 100%;
        align-items: center;
        flex-wrap: wrap;
        span{
            font-size: 1.5rem;
            font-family: Arial, Helvetica, sans-serif;
        }
    .flex{
        display: flex;
        justify-content: center;
        // .btn div{
        //     background-color: blue;
        //     font-family: Arial, Helvetica, sans-serif;
        // }
    }
    }
}
</style>