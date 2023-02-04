<script>
import AppHeaderLinks from './AppHeaderLinks.vue';
export default {
    name: 'AppHeader',
    components: {
        AppHeaderLinks,
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
                    <AppHeaderLinks/>
                </div>
            </div>

        </div>
    </header>

</template>

<style lang="scss" scoped>
header {
    height: $height_header;
    position: sticky;
    top: 0;
    background-color: white;
    z-index: 10;
}

.header_container {
    height: 100%;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .header_logo {
        height: 100%;
        padding: 20px;

        img {
            height: 100%
        }

    }

    .header_links {
        height: 100%;


    }
}
</style>
