<template>
    <div class="d-flex flex-column align-items-start ">
        <div class="text-uppercase mb-3">
            <h3>{{ title }}</h3>
        </div>
        <ul>
            <li v-for="(item, index) in items" :key="index">
                <a class="text-capitalize" :href="item.path">{{ item.name }}</a>
            </li>
        </ul>
    </div>
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
ul {
    padding-left: 0;
}
h3 {
    color: white;
    margin-top: 2rem;
    }
</style>