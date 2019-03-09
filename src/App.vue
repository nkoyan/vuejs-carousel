<template>
    <div>
        <carousel>
            <carousel-slide
                :key="n"
                v-for="n in slides"
                :img="`http://lorempixel.com/630/300/cats/${n}/`"
                text="Salut les gens"
                :index="n - 1"
            >
            </carousel-slide>
        </carousel>
        <button @click.prevent="addSlide">Ajouter un slide</button>
        <button @click.prevent="removeSlide">Enlever un slide</button>
    </div>
</template>

<script>
    import Carousel from './components/carousel/Carousel'
    import CarouselSlide from './components/carousel/CarouselSlide'

    export default {
        name: 'app',
        components: { Carousel, CarouselSlide },
        data () {
            return {
                slides: 5
            }
        },
        methods: {
            addSlide () {
                this.slides++
            },
            removeSlide () {
                if (this.slides > 1) {
                    this.slides--
                }
            }
        }
    }
</script>

<style src="./app.css"></style>