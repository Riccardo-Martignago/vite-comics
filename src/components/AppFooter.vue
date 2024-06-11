<script>
    export default {
        data() {
            return {
                socials:[
                    'footer-facebook.png',
                    'footer-periscope.png',
                    'footer-pinterest.png',
                    'footer-twitter.png',
                    'footer-youtube.png'
                ]
            }
        }
    }
</script>

<template>
    <footer>
        <section class="bg-dc-img">
            <div class="container">
                ciao
            </div>
        </section>
        <section class="bg-gray">
            <div class="container">
                <button>SING-UP NOW!</button>
                <ul>
                    <li>
                        <h2 class="blue">FOLLOW US</h2>
                    </li>
                    <li v-for="item in socials">
                        <img :src="'src/assets/img/'+ item" alt="item">
                    </li>
                </ul>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    .bg-dc-img{
            background-image: url(../assets/img/footer-bg.jpg);
        }
    .bg-gray{
        background-color: #2f3031;
    }
    .blue{
        color: #0282f9
    }
    .container{
        display: flex;
        justify-content: space-between
    }
    button{
        border-color: #0282f9;
        background-color: transparent;
        color: white;
        padding: .8rem .5rem;
    }
    ul{
        @include flex();
        li{
            padding-left: 1rem;
        }
    }
</style>