<script>
export default {
    data() {
        return {
            img:[
                {
                    nome:'buy-comics-digital-comics.png',
                    titolo:'DIGITAL COMICS'
                },
                {
                    nome:'buy-comics-merchandise.png',
                    titolo:'DC MERCHANDISE'
                },
                {
                    nome:'buy-comics-subscriptions.png',
                    titolo:'SUBSCRIPTION'
                },
                {
                    nome:'buy-comics-shop-locator.png',
                    titolo:'COMIC SHOP LOCATOR'
                },
                {
                    nome:'buy-dc-power-visa.svg',
                    titolo:'DC POWER VISA'
                }
            ]
        }
    }
}
</script>

<template>
    <main>
        <section class="bg-black">
            <div class="container">
                <h2>--> Content goes here <--</h2>
            </div>
        </section>
        <section class="bg-blue">
            <div class="container around">
                <article v-for="item in img">
                    <img :src="'src/assets/img/' + item.nome" :alt="item">
                    <p>{{ item.titolo }}</p>
                </article>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/mixins' as *;
    main{
        section{
            color: white;
            div{
                h2{
                    padding: 3rem 0;
                }
            }
        }
    }
    .bg-black{
        background-color: #1c1c1c;
    }
    .bg-blue{
        background-color: #0282f9;
    }
    article, .container{
        display: flex;
    }
    article{
        align-items: center;
        padding: 2rem;
    }
    .around{
        justify-content: space-around;
    }
</style>