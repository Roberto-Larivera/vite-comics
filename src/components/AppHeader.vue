<script>
export default {
    name: 'AppHeader',
    components: {

    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="header_container">
                <div class="header_logo">
                    <img src="../assets/img/dc-logo.png">
                </div>
                <div class="header_links">
                    <ul>
                        <li>
                            <a href="#">characters</a>
                        </li>
                        <li>
                            <a href="#">comics</a>
                        </li>
                        <li>
                            <a href="#">movies</a>
                        </li>
                        <li>
                            <a href="#">tv</a>
                        </li>
                        <li>
                            <a href="#">games</a>
                        </li>
                        <li>
                            <a href="#">collectibles</a>
                        </li>
                        <li>
                            <a href="#">videos</a>
                        </li>
                        <li>
                            <a href="#">fans</a>
                        </li>
                        <li>
                            <a href="#">news</a>
                        </li>
                        <li>
                            <a href="#">shop</a>
                        </li>
                    </ul>
                </div>
            </div>

        </div>
    </header>

</template>

<style lang="scss" scoped>
header {
    height: 150px;
    //padding: 15px;
}

.header_container {
    height: 100%;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.header_logo{
    height: 100%;
    img{
        height: 100%;
    }
}
.header_links {
    height: 100%;

    ul {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;

        li {
            list-style-type: none;
            padding: 10px;
            height: 100%;
            display: flex;
            align-items: center;

            a {
                text-decoration: none;

            }
        }
    }
}
</style>
