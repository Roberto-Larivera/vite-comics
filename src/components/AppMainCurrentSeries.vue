<script>
import AppMainCurrentCard from './AppMainCurrentCard.vue';
import AppMainCardInfo from './AppMainCardInfo.vue';
export default {
    name: 'AppMainCurrentSeries',
    components: {
        AppMainCurrentCard,
        AppMainCardInfo,
    },
    data() {
        return {
            currentBook: 0,
            visibleInfo: false,
            seriesData: [
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    },
    methods: {
        openInfo(index){
            this.currentBook = index;
            this.visibleInfo = true;
        }
    },
}
</script>

<template>
    <div class="main_current__series">
        <div v-if="visibleInfo == false">
            <div class="container">
                <div class="title-section">
                    <h2>current series</h2>
                </div>
                <div class="series_cards">
                    <AppMainCurrentCard :src="element.thumb" :title="element.series" v-for="(element, index) in seriesData" @click="openInfo(index)" />
                </div>
                <button>load more</button>
            </div>
        </div>
        <div v-if="visibleInfo == true">
            <div class="container">
                <AppMainCardInfo :src="seriesData[currentBook].thumb" :title="seriesData[currentBook].series"
                    :price="seriesData[currentBook].price" :type="seriesData[currentBook].type" />
            </div>

        </div>
    </div>
</template>

<style lang="scss" scoped>
.main_current__series {
    min-height: 300px;
    background-color: $bg_main-current--series;
    padding: 50px 0 50px 0;
    text-align: center;

    .container {
        position: relative;

        .title-section {
            display: inline-block;
            background-color: $color_primary;
            padding: 15px;
            position: absolute;
            top: -80px;
            left: 0;

            h2 {
                text-transform: uppercase;
                color: $txt_light-primary;
                font-weight: 900;
            }
        }
    }

    .series_cards {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
        width: 100%;
        margin-bottom: 20px;


    }

    button {
        @include button ($color_primary, $bttn_light-primary, $bg_main-current--series, $color_primary, 10px 50px 10px 50px, uppercase, 700, $color_primary)
    }
}
</style>
