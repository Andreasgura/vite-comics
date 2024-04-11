<template>
    <div class="text-uppercase">
        {{ title }}
    </div>

    <ul>
        <li v-for="(item, index) in items" :key="index">
            <a :href="item.path">{{ item.name }}</a>
        </li>
    </ul>
</template>

<script>
    export default {
        name: 'MenuComponent',
        props: {
            title: String,
            items: Array
        },
        
    }
</script>

<style lang="scss" scoped>

</style>