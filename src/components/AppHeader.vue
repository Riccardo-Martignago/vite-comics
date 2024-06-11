<script>
export default {
    data() {
        return {
            menu:[
                'characters',
                'comics',
                'movies',
                'tv',
                'games',
                'collectibles',
                'videos',
                'fans',
                'news',
                'shop'
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <section>
                <img src="../assets/img/dc-logo.png" alt="">
                <nav>
                    <ul>
                        <li v-for="item in menu" :key="item.id">
                            <a href="">{{ item }}</a>
                        </li>
                    </ul>
                </nav>
            </section>
        </div>
    </header>
</template>

<style lang="scss"scoped>
section{
    display: flex;
    justify-content: space-between;
    align-items: center;
    img{
        padding: 1rem 0;
    }
}
ul{
    display: flex;
    li{
        padding: 1rem;
        a{
            text-decoration: none;
            color: black;
        }
        a:hover{
            color: #0282f9;
            border-bottom: 3px solid #0282f9;
            padding-bottom: 3rem;
        }
    }
}

</style>