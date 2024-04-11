<template>
    <main>
        <div class="container">

            <div class="row">
                <ComicsCard v-for="(comic, index) in comics" :key="index" :img="comic.thumb"
                    :description="comic.series" 
                />
            </div>

        </div>
    </main>
</template>

<script>
import ComicsCard from './ComicsCard.vue';
import { comics } from '../data/store.js';
export default {
    name: 'MainComponent',
    components: {
        ComicsCard,
    },
    data() {
        return {
            comics,
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../assets/styles/partials/variables' as *;

main {
    background-color: $mainbg;
    color: white;
    padding: 50px 0;
}
</style>