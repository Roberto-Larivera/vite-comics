<script>
export default {
    name: 'AppFooterButtonLinks',
    components: {

    }
}
</script>

<template>
    <div class="content_links">
        <ul>
            <li>
                <a href="#nogo">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt=""> <!--target="_blank"-->
                    <span>digital comics</span>
                </a>
            </li>
            <li>
                <a href="#nogo">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    <span>dc merchandise</span>
                </a>
            </li>
            <li>
                <a href="#nogo">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    <span>subscription</span>
                </a>
            </li>
            <li>
                <a href="#nogo">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    <span>comic shop locator</span>
                </a>
            </li>
            <li>
                <a href="#nogo">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    <span>dc power visa</span>
                </a>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
.content_links {
    height: 100%;
    width: 100%;


    ul {
        @include displayFlex (space-around);
        height: 100%;
        width: 100%;

        li {
            list-style-type: none;
            padding: 10px;
            height: 100%;
            @include displayFlex (flex-start);

            &:hover {
                background-color: rgba(255, 255, 255, 0.1);
            }

            a {

                text-decoration: none;
                color: white;
                text-transform: uppercase;
                font-weight: 300;

                img {
                    vertical-align: middle;
                    height: 50px;
                    width: 50px;
                    object-fit: contain;
                    margin-right: 10px;
                }

                span {
                    vertical-align: middle;
                    font-size: .8rem;
                }
            }
        }
    }
}
</style>
