<template>
    <div>

        <div>
            <h3 class="text-uppercase mb-3">{{ title }}</h3>
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
@use '../../assets/styles/partials/variables' as *;

ul {
    padding-left: 0;
}

h3 {
    color: white;
    margin-top: 2rem;
}

a {
    color: $links;
}
</style>