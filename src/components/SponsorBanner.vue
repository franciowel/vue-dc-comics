<template>
    
    <div class="jumbosponsor">
        <div class="contain">
            <a  class="btn" href="">
                CURRENT SERIES
            </a>
        </div>
    </div>

</template>

<script>
export default {
    name: 'SponsorBanner'
}
</script>

<style lang="scss" scoped>
@import '../style/color.scss';
@import '../style/commons.scss';
@import '../style/font.scss';

.jumbosponsor{
    background-image: url(../assets/img/jumbotron.jpg);
    height: 450px;
    position: relative;
}

.btn{
    background-color: $primary;
    font-family: $similfont;
    padding: 1rem 1.5rem;
    color: white;
    font-weight: 600;
    bottom: -1.5rem;
    position: absolute;
}


</style>