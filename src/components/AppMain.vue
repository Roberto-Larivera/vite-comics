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
                        --> Content goes here &lt;--
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
                                digital comics
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                dc merchandise
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                subscription
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                comic shop locator
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                dc power visa
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>

    </main>
</template>

<style lang="scss">
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

                a {
                    text-decoration: none;
                    color: white;
                }
            }
        }
    }
}
</style>
