<script>
export default {
    name: 'AppMainCurrentCard',
    components: {

    },
    props: {
        src: String,
        title: String

    },
}
</script>

<template>
    <div class="card">
        <div class="card_image">
            <img :src="src" :alt="title">
        </div>
        <h3>{{ title }}</h3>
    </div>
</template>

<style lang="scss" scoped>
.card {
    width: calc((100% / 6));
    padding: 5px;
    margin-bottom: 20px;

    .card_image {
        width: 100%;

        img {
            width: 100%;
            object-fit: cover;
            object-position: center;
            aspect-ratio: 1;

        }
    }

    h3 {
        color: $txt_light-primary;
        font-weight: 700;
        margin-top: 15px;
        text-transform: capitalize;
    }
}
</style>
