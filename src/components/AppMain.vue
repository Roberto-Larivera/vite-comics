<script>
import AppMainJumbotron from "./AppMainJumbotron.vue"
import AppMainCurrentSeries from "./AppMainCurrentSeries.vue"

export default {
    name: 'AppMain',
    components: {
        AppMainJumbotron,
        AppMainCurrentSeries,
    },
}
</script>

<template>
    <main>
        <AppMainJumbotron/>
        <AppMainCurrentSeries/>
        
        <!-- <div class="main_content">
            <div class="container">
                <div class="content_title">

                    <h2>
                        --&gt; Content goes here &lt;--
                    </h2>
                </div>
            </div>
        </div> -->

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

</style>
