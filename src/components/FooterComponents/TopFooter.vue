<template>
    <div id="top-footer">
        <div class="container">
            <ul class="d-flex flex-row py-3">
                <li class="d-flex flex-row" v-for="(page, index) in pages" :key="index">
                    <TfCard :img="page.imgpath" :description="page.name" />
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
import TfCard from './TfCard.vue';
import {pages} from '../../data/store.js';

export default {
    name: 'TopFooter',
    components: {
        TfCard
    },
    data() {
        return {
            pages: pages,
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
ul{
    margin-bottom: 0;
}
</style>