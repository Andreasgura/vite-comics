<template>
    <div class="d-flex align-items-center gap-2">
        <div class="w-25 ">
            <img :src="img" :alt="description"
            class="w-100">
        </div>
        <div class="text-uppercase ">
            {{ description }}
        </div>
    </div>
</template>

<script>
export default {
    name: 'TfCard',
    props: {
        img: String,
        description: String
    }
}
</script>

<style lang="scss" scoped></style>