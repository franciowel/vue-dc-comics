<template>
    
    <section class="background">

        <div class="contain">

            <div class="flexcontain">

                <div class="sign-up">
                    <a href="#">
                        SIGN UP NOW!
                    </a>
                </div>

                <div class="flexcontain">

                    <div class="text">
                        FOLLOW US!
                    </div>

                    <div class="flexcontain social-links">

                        <a href="#">
                            <img src="../assets/img/footer-facebook.png" alt="Facebook">
                        </a>

                        <a href="#">
                            <img src="../assets/img/footer-periscope.png" alt="Periscope">
                        </a>

                        <a href="#">
                            <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
                        </a>

                        <a href="#">
                            <img src="../assets/img/footer-twitter.png" alt="Twitter">
                        </a>

                        <a href="#">
                            <img src="../assets/img/footer-youtube.png" alt="Youtube">
                        </a>
                    </div>
                </div>

            </div>
        </div>

    </section>

</template>

<script>
export default {
    name: 'FooterBottom'
}
</script>

<style lang="scss" scoped>
@import url('../style/commons.scss');
@import url('../style/font.scss');

.background{
    background-color: #303030;
    font-family: Arial, Helvetica, sans-serif;
    height: 120px;
    color: white;
    .contain{
    height: 100%;
    }
    .flexcontain{
        justify-content: space-between;
        align-items: center;
        height: 100%;
    }
    .sign-up{
        border: solid #2481f4 1px;
        padding: 0.8rem 2rem;
    }
    .text{
        font-weight: 600;
        font-size: 1.4rem;
        color: #2481f4;
    }
    .social-links a{
        margin: 0.5rem;
    }
}
</style>
