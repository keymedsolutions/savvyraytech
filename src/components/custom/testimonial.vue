<template>
    <div class="slick-space-gutter--15 rn-slick-dot rn-slick-arrow mb--60">
        <VueSlickCarousel v-bind="sliderSetting">
            <div v-for="(item, index) in testimonial" :key="index">
                 <div class="rn-box-card card-style-default testimonial-style-one">
                    <div class="inner">
                        <figure class="thumbnail">
                            <img :src="require(`@/assets/images/testimonial/${item.image}`)"
                                alt="Testimonial image"/>
                        </figure>
                        <figcaption class="content">
                            <p class="description">{{ item.description }}</p>
                            <h2 class="title">{{ item.name }}</h2>
                            <h6 class="subtitle theme-gradient">{{ item.designation }}</h6>
                        </figcaption>
                    </div>
                </div>
            </div>
        </VueSlickCarousel>
    </div>
</template>

<script>
    import VueSlickCarousel from 'vue-slick-carousel'

    export default {
        name: 'Testimonial',
        components: {VueSlickCarousel},
        props: {
            testimonial: {},
        },
        data() {
            return {
                sliderSetting: {
                    infinite: true,
                    slidesToShow: 2,
                    slidesToScroll: 1,
                    dots: true,
                    arrows: true,
                    responsive: [
                        {
                            breakpoint: 800,
                            settings: {
                                slidesToShow: 2,
                            }
                        },
                        {
                            breakpoint: 993,
                            settings: {
                                slidesToShow: 2,
                            }
                        },
                        {
                            breakpoint: 580,
                            settings: {
                                slidesToShow: 1,
                            }
                        },
                        {
                            breakpoint: 481,
                            settings: {
                                slidesToShow: 1,
                            }
                        }
                    ]
                }
            }
        }
    }
</script>