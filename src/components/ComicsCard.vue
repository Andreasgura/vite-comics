<template>
    <div class="col-12 col-md-6 col-lg-2 mb-3 ">
        <div class="mb-3">
            <img class="w-100"
            :src="img" :alt="description">
        </div>
        <div class="text-uppercase ">
            {{ description }}
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ComicsCard',
        props: {
            img: String,
            description: String
        }
    }
</script>

<style lang="scss" scoped>
img {
    aspect-ratio: 1/1;
    object-fit: cover;
}
</style>