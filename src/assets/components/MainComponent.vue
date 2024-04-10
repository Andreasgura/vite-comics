<template>
    <main>
        <div class="container">
            - ->Content goes here<- -
        </div>
    </main>
</template>

<script>
    export default {
        name: 'MainComponent',
    }
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
    main {
        background-color: $mainbg;
        color: white;
        padding: 50px 0;
    }
</style>