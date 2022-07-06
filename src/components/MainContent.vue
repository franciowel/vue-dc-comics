<template>
    <div class="color">
        <div class="contain flexcontain">
            <span>Contents will go Here!</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MainContent'
}
</script>

<style lang="scss" scoped>
@import '../style/color.scss';
.color{
    background-color: #1c1c1c;
    color: white;
    height: 150px;
    .contain{
        height: 100%;
        align-items: center;
        span{
            font-size: 1.5rem;
            font-family: Arial, Helvetica, sans-serif;
        }
    }
}
</style>