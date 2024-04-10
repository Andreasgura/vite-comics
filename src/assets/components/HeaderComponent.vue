<template>
    <header>
        <div class="container py-4 ">
            <div class="d-flex justify-content-between">
                <div><img src="/img/dc-logo.png" alt="logo"></div>
                <div class="d-flex align-items-center">
                    <ul class="text-uppercase d-flex h-100">
                        <li class="d-flex align-items-center" v-for="(anchores, index) in anchores" :key="index">
                            <a :href="anchores.path">{{ anchores.name }}</a>
                        </li>
                    </ul>

                </div>
            </div>
        </div>
    </header>
</template>

<script>
    export default {
        name: 'HeaderComponent',
        data () {
            return {
                anchores: [
                    {
                        name: 'characters',
                        path: '#'
                    },
                    {
                        name: 'comics',
                        path: '#'
                    },
                    {
                        name: 'movies',
                        path: '#'
                    },
                    {
                        name: 'tv',
                        path: '#'
                    },
                    {
                        name: 'games',
                        path: '#'
                    },
                    {
                        name: 'collectibles',
                        path: '#'
                    },
                    {
                        name: 'videos',
                        path: '#'
                    },
                ]
            }
        },
        
    }
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

header {
    background-color: $headerbg;
    
    li {
        border-bottom: 3px solid transparent;
        margin: 0 10px;
        align-items: center;
        &:hover {
            border-bottom: 3px solid $headeranchorover;
            a {
                color: $headeranchorover;
            }
        }
    }
        a {
            color: black;
            
            font-weight: bold;
           
        }
    
}
</style>