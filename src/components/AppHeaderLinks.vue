<script>
export default {
    name: 'AppHeaderLinks',
    components: {

    },
    data() {
        return {
            currentLinks: 0,
            links: [
                {
                    txt: 'characters',
                    link: '#nogo',
                    status: false,
                },
                {
                    txt: 'comics',
                    link: '#nogo',
                    status: false,
                },
                {
                    txt: 'movies',
                    link: '#nogo',
                    status: false,
                },
                {
                    txt: 'tv',
                    link: '#nogo',
                    status: false,
                },
                {
                    txt: 'games',
                    link: '#nogo',
                    status: false,
                },
                {
                    txt: 'collectibles',
                    link: '#nogo',
                    status: false,
                },
                {
                    txt: 'videos',
                    link: '#nogo',
                    status: false,
                },
                {
                    txt: 'fans',
                    link: '#nogo',
                    status: false,
                },
                {
                    txt: 'news',
                    link: '#nogo',
                    status: false,
                },
                {
                    txt: 'shop',
                    link: '#nogo',
                    status: false,
                },
            ]

        }
    },
    methods: {
        menuMesssageOpenList(item, x){
            if(this.links[this.currentLinks].status == true && this.links[this.currentLinks] != item){
                this.links[this.currentLinks].status = false;
                item.status = !item.status
            }
            else if(this.links[this.currentLinks] == item){
                item.status = !item.status
            }
            else{
                item.status = !item.status
            }
            this.currentLinks = x ;
            
        }
    },
}
</script>

<template>
    <div>
        <ul>
            <li v-for="item,index in links" :class="(item.status==true)? 'active':''" >
                <a :href="item.link" @click="menuMesssageOpenList(item, index)">{{ item.txt }}</a>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
div{
    height: 100%;
}
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

        &.active,
        &:hover {
            box-shadow: inset 0px -6px 0px 0px $color_primary;
        }

        &.active a,
        &:hover a {
            color: $color_primary;
        }

        a {
            text-decoration: none;
            text-transform: uppercase;
            font-weight: bold;
            color: $txt_link;
        }
    }
}
</style>
