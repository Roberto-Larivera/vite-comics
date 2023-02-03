<script>
export default {
    name: 'AppFooter',
    components: {

    }
}
</script>

<template>
    <footer>
        <div class="footer_top">
            <div class="container">
                <div class="top_content">
                    <div class="top_content-links">
                        <div class="content_links-left">
                            <h3>
                                dc comics
                            </h3>
                            <ul>
                                <li>
                                    <a href="#">
                                        Characters
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Comics
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Movies
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        TV
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Games
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Videos
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        News
                                    </a>
                                </li>
                            </ul>
                            <h3>
                                shop
                            </h3>
                            <ul>
                                <li>
                                    <a href="#">
                                        Shop DC
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Shop DC Collectibles
                                    </a>
                                </li>
                            </ul>
                        </div>
                        <div class="content_links-center">
                            <h3>
                                dc
                            </h3>
                            <ul>
                                <li>
                                    <a href="#">
                                        Terms Of Use
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Privacy policy (New)
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Ad Choices
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Advertising
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Jobs
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Subscriptions
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Talent Workshops
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        CPSC Certificates
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Ratings
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Shop Help
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        Contact Us
                                    </a>
                                </li>
                            </ul>
                        </div>
                        <div class="content_links-right">
                            <h3>
                                sites
                            </h3>
                            <ul>
                                <li>
                                    <a href="#">
                                        DC
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        MAD Magazine
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        DC Kids
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        DC Universe
                                    </a>
                                </li>
                                <li>
                                    <a href="#">
                                        DC Power Visa
                                    </a>
                                </li>
                            </ul>
                        </div>
                        <div class="top_content-logo">
                        </div>

                    </div>
                </div>
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
                                <a href="#">
                                    <img src="../assets/img/footer-facebook.png" alt="icon-facebook">
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <img src="../assets/img/footer-twitter.png" alt="icon-twitter">
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <img src="../assets/img/footer-youtube.png" alt="icon-youtube">
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    <img src="../assets/img/footer-pinterest.png" alt="icon-pinterest">
                                </a>
                            </li>
                            <li>
                                <a href="#">
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
        width: 100%;
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;

        .container {
            background-image: url(../assets/img/dc-logo-bg.png);
            background-repeat: no-repeat;
            // background-size: cover;
            background-position: right;

        }

        .top_content {
            height: 100%;
            width: 100%;

            .top_content-links {
                padding-top: 20px;
                padding-bottom: 20px;
                height: 100%;
                display: flex;

                .content_links-left,
                .content_links-center,
                .content_links-right {
                    margin-right: 20px;

                    h3 {
                        color: $txt_light-primary;
                        margin-top: 20px;
                        margin-bottom: 20px;
                        text-transform: uppercase;
                    }

                    ul {
                        width: 100%;

                        li {
                            list-style-type: none;
                            height: 100%;
                            margin-bottom: 5px;
                            display: flex;
                            align-items: center;

                            a {
                                text-decoration: none;
                                color: $txt_link;
                                text-transform: capitalize;
                            }
                        }
                    }
                }
            }
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
