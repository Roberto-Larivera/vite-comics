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
                <h2>{{ title }}</h2>
                <p>{{ type }}</p>
                <span>{{ price }}</span>
            </div>
            <div>
                <div>
                    <button class="my-btn-buy">acquista</button>
                </div>
                <div>
                    <button class="my-btn-end" >indietro</button>
                </div>
            </div>
        </div>

    </div>
</template>

<style lang="scss" scoped>
.section_info {
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

        p {
            margin-bottom: 20px;
            text-transform: capitalize;
        }

        span {
            color: green;
            font-weight: 900;
            font-size: 1.3rem;
            margin-bottom: 20px;
        }
        button.my-btn-buy{
                @include button(green,$bttn_light-primary,green,green);
                margin: 20px 0;
            }
        
        button.my-btn-end{
            @include button(red,$bttn_light-primary,red,red);
        }
    }
}
</style>
