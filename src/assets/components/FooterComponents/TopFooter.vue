<template>
    <div id="top-footer">
        <div class="container">
            <ul class="d-flex flex-row py-3">
                <li class="d-flex flex-row"
                v-for="(page, index) in pages" :key="index">
                    <TfCard :img="page.imgpath" :description="page.name"/>    
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
import TfCard from './TfCard.vue'
    export default {
        name : 'TopFooter',
        components: {
            TfCard
        },
        data () {
            return {
                pages : [
                    {
                        imgpath: '/img/buy-comics-digital-comics.png',
                        name: 'digital comics'
                    },
                    {
                        imgpath: '/img/buy-comics-merchandise.png',
                        name: 'merchandise'
                    },
                    {
                        imgpath: '/img/buy-comics-subscriptions.png',
                        name: 'subscriptions'
                    },
                    {
                        imgpath: '/img/buy-comics-shop-locator.png',
                        name: 'shop locator'
                    },
                    {
                        imgpath: '/img/buy-dc-power-visa.svg',
                        name: 'dc power visa'
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
@use '/src/assets/styles/partials/variables' as *;
#top-footer {
    background-color: $topfooterbg;
    color: white;
}
li {
    div {
        padding: 5px;
    }
}
</style>