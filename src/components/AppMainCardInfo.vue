<script>
export default {
    name: 'AppMainCardInfo',
    components: {

    },
    props: {
        src: String,
        title: String,
        price: String,
        type: String,

    },
}
</script>

<template>
    <div class="section_info">

        <div class="info_image">
            <img :src="src" :alt="title">
        </div>
        <div class="info_serie">
            <div>
                <h2>{{title}}</h2>
            <p>{{type}}</p>
            <span>{{price}}</span>
        </div>
            <button>acquista</button>
        </div>

    </div>
</template>

<style lang="scss" scoped>
.section_info{
    @include displayFlex();
    height: 100%;
    .info_image {
        width: 30%;
    
        img {
            width: 100%;
        }
    }
    
    .info_serie {
        width: 70%;
        height: 100%;

        @include displayFlex();
        flex-direction: column;
        color: $txt_light-primary;

}
}
</style>
