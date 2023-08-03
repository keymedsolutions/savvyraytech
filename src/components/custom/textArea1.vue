<template>
    <div class="rwt-about-area rn-section-gap">
        <div class="container">
            <div class="row row--30 align-items-center">
                <div class="col-lg-6">
                    <div class="thumbnail" data-aos="fade-up" data-aos-delay="250">
                        <img class="w-100" src="../../assets/images/home/home-photo1.png" alt="Teams. ">
                    </div>
                </div>
                <div class="col-lg-6 mt_md--40 mt_sm--40">
                    <div class="content">
                        <div class="section-title">
                            <h4 class="subtitle" data-aos="fade-up" data-aos-delay="280">
                                <span class="theme-gradient">We are more than just a marketing agency</span>
                            </h4>
                            <h2 class="title mt--10" data-aos="fade-up" data-aos-delay="310">About Our Business</h2>
                            <p data-aos="fade-up" data-aos-delay="310">
                                Savvy Ray Technologies is a digital advertising agency made up of enthusiastic people that have come together to help your achievement in business. Every project can become a success story because we have the resources and the motivation to make it so. For us to build genuine connections with the businesses of our clients, we strive to create digital experiences that interact and engage with end users. Our aim is to offer our customers value that is outstanding, to make their online experience satisfying, and to transform their digital platform to become a location where the business may grow tremendously.
                            </p>
                            <!-- <ul class="list-icon" data-aos="fade-up" data-aos-delay="340">
                                <li>
                                    <Icon name="check" size="20" icon-class="icon d-inline-flex align-items-center justify-content-center"/>
                                    Track your teams progress with mobile app.
                                </li>
                                <li>
                                    <Icon name="check" size="20" icon-class="icon d-inline-flex align-items-center justify-content-center"/>
                                    Lorem ipsum dolor sit amet consectetur adipisicing.
                                </li>
                                <li>
                                    <Icon name="check" size="20" icon-class="icon d-inline-flex align-items-center justify-content-center"/>
                                    Ipsum dolor sit amet consectetur adipisicing.
                                </li>
                                <li>
                                    <Icon name="check" size="20" icon-class="icon d-inline-flex align-items-center justify-content-center"/>
                                    Your teams progress with mobile app.
                                </li>
                            </ul> -->

                            <!-- <div class="read-more-btn mt--40" data-aos="fade-up" data-aos-delay="370">
                                <router-link class="btn-default btn-icon"
                                   to="/about">
                                    More About Us
                                    <Icon name="arrow-right" size="20" icon-class="icon"/>
                                </router-link>
                            </div> -->
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <homepageAccordian/>

    </div>
</template>

<script>
    import Icon from '../icon/Icon'
    import Accordion from '../elements/accordion/Accordion'
    import homepageAccordian from "../../components/custom/homepageAccordian";


    export default {
        name: 'TextArea1',
        components: {Icon, Accordion, homepageAccordian}
    }
</script>