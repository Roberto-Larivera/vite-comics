<script>
import AppFooterButtonLinks from './AppFooterButtonLinks.vue';
import AppFooterListLinks from './AppFooterListLinks.vue';
export default {
    name: 'AppFooter',
    components: {
        AppFooterButtonLinks,
        AppFooterListLinks,
    }
}
</script>

<template>
    <footer>
        <div class="footer_top">
            <div class="container">
                <AppFooterButtonLinks/>
                
            </div>
        </div>
        <div class="footer_center multi-bg">
            <div class="container">
                <AppFooterListLinks/>
            </div>
        </div>
        <div class="footer_bottom">
            <div class="container">
                <div class="bottom_content">
                    <div class="bottom_content-start">
                        <button>sign-up now!</button>
                    </div>
                    <div class="bottom_content-end">

                        <ul>
                            <li>
                                <span>follow us</span>
                            </li>
                            <li>
                                <a href="#nogo">
                                    <img src="../assets/img/footer-facebook.png" alt="icon-facebook">
                                </a>
                            </li>
                            <li>
                                <a href="#nogo">
                                    <img src="../assets/img/footer-twitter.png" alt="icon-twitter">
                                </a>
                            </li>
                            <li>
                                <a href="#nogo">
                                    <img src="../assets/img/footer-youtube.png" alt="icon-youtube">
                                </a>
                            </li>
                            <li>
                                <a href="#nogo">
                                    <img src="../assets/img/footer-pinterest.png" alt="icon-pinterest">
                                </a>
                            </li>
                            <li>
                                <a href="#nogo">
                                    <img src="../assets/img/footer-periscope.png" alt="icon-periscope">
                                </a>
                            </li>
                        </ul>

                    </div>

                </div>
            </div>
        </div>

    </footer>
</template>

<style lang="scss" scoped>
footer {
    .footer_top {
    background-color: #0282F9;
    height: 150px;
    width: 100%;

    
}
    .footer_center {
        width: 100%;
        background-image:url(../assets/img/footer-bg.jpg);
        background-repeat:no-repeat;
        background-size: cover;
        background-position: center;

        // UTILIZZO SFONDO DOPPIO
        /*
        // &.multi-bg{
        //     background-image: url('../assets/img/dc-logo-bg.png'),url('../assets/img/footer-bg.jpg');
        //     background-repeat: no-repeat, no-repeat;
        //     background-size: none, cover;
        //     background-position: right, center;
        // }
        */
        .container {
            background-image: url(../assets/img/dc-logo-bg.png);
            background-repeat: no-repeat;
            // background-size: cover;
            background-position: right;

        }

        
    }

    .footer_bottom {
        height: $height_foot-bottom;
        width: 100%;
        background-color: #303030;

        .bottom_content {
            height: 100%;
            width: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;

            .bottom_content-start {
                // button {
                //     padding: 10px;
                //     text-transform: uppercase;
                //     background-color: transparent;
                //     border: 2px solid $color_primary;
                //     color: $bttn_light-primary;

                //     &:hover {
                //         background-color: $color_primary;
                //     }
                // }
                button{
                    @include button ($color_primary,$bttn_light-primary,$color_primary,$color_primary)
                }
            }

            .bottom_content-end {
                ul {
                    display: flex;
                    justify-content: space-around;
                    align-items: center;
                    height: 100%;
                    width: 100%;

                    li {
                        list-style-type: none;
                        padding: 10px;
                        height: 100%;
                        display: flex;
                        align-items: center;


                        span {
                            text-transform: uppercase;
                            color: $color_primary;
                            font-weight: 900;

                        }

                        a {
                            text-decoration: none;
                            color: $txt_light-primary;
                        }
                    }
                }
            }
        }
    }
}
</style>
