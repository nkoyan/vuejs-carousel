<template>
    <div>
        <carousel>
            <carousel-slide
                text="Salut les gens"
                img="http://lorempixel.com/630/300/cats/1/"
            >
            </carousel-slide>
            <carousel-slide
                text="Aurevoir les gens"
                img="http://lorempixel.com/630/300/cats/2/"
            >
            </carousel-slide>
            <carousel-slide
                text="Aurevoir les gens"
                img="http://lorempixel.com/630/300/cats/3/"
            >
            </carousel-slide>
        </carousel>
    </div>
</template>

<script>
    import Carousel from './components/carousel/Carousel'
    import CarouselSlide from './components/carousel/CarouselSlide'

    export default {
        name: 'app',
        components: { Carousel, CarouselSlide }
    }
</script>

<style src="./app.css"></style>