<template>
    <div>
        <MenuComponent :title="dcMenu.title" :items="dcMenu.menu"/>
    </div>
</template>

<script>
    import {dcMenu} from '../../data/store.js';
    import MenuComponent from '../FooterComponents/MenuComponent.vue';
    export default {
        name : 'MainFooter',
        components: {
            MenuComponent,
        },
        data() {
            return {
                dcMenu,
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>