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

                    </div>
                    <div class="top_content-logo">

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

<style lang="scss">
footer {
    .footer_bottom {
        height: 150px;
        width: 100%;
        background-color: #303030;

        .bottom_content {
            height: 100%;
            width: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;

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

                    a {
                        text-decoration: none;
                        color: white;
                    }
                }
            }
        }
    }
}
</style>
