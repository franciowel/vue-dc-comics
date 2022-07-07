<template>
    <div class="card">
        <div class="img-container">
            <img :src="comicDetails.thumb" :alt="comicDetails.series">
        </div>
        <p>{{ comicDetails.series }}</p>
    </div>
</template>

<script>
export default {
    name: 'ContentCards',
    props: {
        comicDetails: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../style/font.scss';

p {
    margin-top: 20px;
    font-family: $similfont;
}
.card {
    width: 190px;
    margin: 15px;
    margin-top: 30px;
    .img-container {
        width: 180px;
        height: 170px;
        overflow: hidden;
    }
}
</style>