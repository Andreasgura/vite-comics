<template>
    <div class="bottom-footer py-3 ">
        <div class="container d-flex justify-content-between">
            <div class="text-uppercase btn-sing-up">
                sing up now!
            </div>
            <div class="d-flex align-items-center gap-3 ">
                <div class="btn-follow text-uppercase">
                    follow us
                </div>
                <div class="d-flex "
                v-for="(icon, index) in icons" :key="index">
                    <img :src="icon.path" :alt="icon.name">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import { icons } from '@/data/store';
export default {
    name: 'BottomFooter'
    , data() {
        return {
            icons
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../../assets/styles/partials/variables' as *;

div.bottom-footer {
    background-color: #303030;
}

div.btn-sing-up {
    border: 1px solid $headeranchorover;
    padding: 10px;
    color: white;
}

div.btn-follow {
    color: #0282F7;
}
div.text-uppercase {
    font-weight: bold;
}
</style>