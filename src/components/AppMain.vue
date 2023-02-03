<script>
export default {
    name: 'AppMain',
    components: {
    }
}
</script>

<template>
    <main>
        <div class="main_content">
            <div class="container">
                <div class="content_title">

                    <h2>
                        --&gt; Content goes here &lt;--
                    </h2>
                </div>
            </div>
        </div>
        <div class="main_content-links">
            <div class="container">
                <div class="content_links">

                    <ul>
                        <li>
                            <a href="#">
                                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                                <span>digital comics</span>
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                                <span>dc merchandise</span>
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                                <span>subscription</span>
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                                <span>comic shop locator</span>
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                                <span>dc power visa</span>
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>

    </main>
</template>

<style lang="scss" scoped>
main {
    height: calc(100% - 150px);
}

.main_content {
    background-color: black;
    height: 150px;
    width: 100%;

    .content_title {
        height: 100%;
        width: 100%;
        display: flex;
        align-items: center;

        h2 {
            color: white;
        }
    }
}

.main_content-links {
    background-color: #0282F9;
    height: 150px;
    width: 100%;

    .content_links {
        height: 100%;
        width: 100%;


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
                &:hover{
                    background-color: rgba(255, 255, 255, 0.1);
                }
                a {
                   
                    text-decoration: none;
                    color: white;
                    text-transform: uppercase;
                    font-weight: 300;
                    img{
                        vertical-align: middle;
                        height: 50px;
                        width: 50px;
                        object-fit: contain;
                        margin-right: 10px;
                    }
                    span{
                        vertical-align: middle;
                        font-size: .8rem;
                    }
                }
            }
        }
    }
}
</style>
