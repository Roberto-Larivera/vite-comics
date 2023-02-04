<script>
export default {
    name: 'AppFooterListLinks',
    components: {

    },
}
</script>

<template>
    <div class="center_content">
        <div class="center_content-links">
            <div class="content_links-left">
                <h3>
                    dc comics
                </h3>
                <ul>
                    <li>
                        <a href="#nogo">
                            Characters
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            Comics
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            Movies
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            TV
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            Games
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            Videos
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            News
                        </a>
                    </li>
                </ul>
                <h3>
                    shop
                </h3>
                <ul>
                    <li>
                        <a href="#nogo">
                            Shop DC
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
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
                        <a href="#nogo">
                            Terms Of Use
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            Privacy policy (New)
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            Ad Choices
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            Advertising
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            Jobs
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            Subscriptions
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            Talent Workshops
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            CPSC Certificates
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            Ratings
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            Shop Help
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
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
                        <a href="#nogo">
                            DC
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            MAD Magazine
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            DC Kids
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            DC Universe
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            DC Power Visa
                        </a>
                    </li>
                </ul>
            </div>
            <div class="center_content-logo">
            </div>

        </div>
    </div>
</template>

<style lang="scss" scoped>
.center_content {
    height: 100%;
    width: 100%;

    .center_content-links {
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

                        &:hover {
                            color: $color_primary;
                            text-decoration:underline;
                        }
                    }
                }
            }
        }
    }
}
</style>
