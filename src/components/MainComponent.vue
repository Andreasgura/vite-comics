<template>
    <div class="jumbo">

    </div>
    <main>

        <div class="container">
            <div class="btn btn-primary text-uppercase">current series</div>
            <div class="row">
                <ComicsCard v-for="(comic, index) in comics" :key="index" :img="comic.thumb"
                    :description="comic.series" />
            </div>
            <div class="d-flex justify-content-center">
                <div class="btn btn-primary text-uppercase mt-5 px-5 ">Load More</div>
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

.jumbo {
    height: 300px;
    background-image: url('/img/jumbotron.jpg');
    background-size: cover;
}

main {
    background-color: $mainbg;
    color: white;

    .btn {
        transform: translateY(-50%);
    }
}

.btn {
    transform: translateY(-50%);
    border-radius: 0;

}
</style>