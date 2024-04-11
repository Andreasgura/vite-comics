<template>
    <div id="mainfooter">
        <div class="container d-flex justify-content-between">
            <div class="d-flex gap-5">
                <div>
                    <MenuComponent :title="dccomicsMenu.title" :items="dccomicsMenu.menu" />
                    <MenuComponent :title="shopMenu.title" :items="shopMenu.menu" />
                </div>
                <MenuComponent :title="dcMenu.title" :items="dcMenu.menu" />
                <MenuComponent :title="sitesMenu.title" :items="sitesMenu.menu" />
            </div>
            <div>
                <img src="/img/dc-logo-bg.png" alt="logo">
            </div>
        </div>
    </div>
</template>

<script>
import { dccomicsMenu, sitesMenu, shopMenu, dcMenu } from '../../data/store.js';
import MenuComponent from '../FooterComponents/MenuComponent.vue';
export default {
    name: 'MainFooter',
    components: {
        MenuComponent,
    },
    data() {
        return {
            dccomicsMenu,
            sitesMenu,
            shopMenu,
            dcMenu
        }
    }
}
</script>

<style lang="scss" scoped>
#mainfooter {
    background-image: url('/img/footer-bg.jpg');
    background-size: cover;
}
</style>