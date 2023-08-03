<template>
    <Layout header-class="header-transparent" buy-button-class="btn-default btn-small">
        <!-- Start Slider Area -->
        <div class="slider-area slider-style-6 shape-right height-750">
            <div class="container">
                <div class="row row--30 align-items-center">
                    <div class="order-2 order-lg-1 col-lg-12 mt_md--50 mt_sm--50 mt_lg--30">
                        <div class="inner text-start">
                            <h1 class="title color-white" data-aos="fade-up" data-aos-delay="100">
                                Transforming businesses in the digital era
                            </h1>
                            <p class="description color-white" data-aos="fade-up" data-aos-delay="150">
                                Ask Savvy Ray Technologies to create a complete and ambitious digital marketing plan that will elevate your business to new levels of success
                            </p>
                            <div class="button-group mt--30 mt_sm--20" data-aos="fade-up" data-aos-delay="200">
                                <a class="btn-default btn-medium btn-icon btn-border"
                                   href="#">
                                    Let's talk <Icon name="arrow-right" size="20" icon-class="icon"/>
                                </a>
                            </div>
                        </div>
                    </div>
                    <!-- <div class="col-lg-6 order-1 order-lg-2">
                        <div class="thumbnail" data-aos="fade-up" data-aos-delay="100">
                            <img src="../../assets/images/banner/banenr-image-02.png" alt="Banner Images"/>
                        </div>
                    </div>
                    <div class="shape-image w-auto">
                        <img src="../../assets/images/banner/white-shape.svg" alt="Banner Images"/>
                    </div> -->
                </div>
            </div>
        </div>
        <!-- End Slider Area -->

        <!-- Start CTA Area -->
        <!-- <CallToAction
            :style-type="6"
            title="Ready to start creating a standard website?"
            btn-text="Purchase Doob"
        /> -->
        <!-- End CTA Area -->

        <Separator/>

        <!-- Start Timeline Area -->
        <div class="rwt-timeline-area rn-section-gap">
            <div class="container">
                <div class="row">
                    <div class="col-lg-12">
                        <SectionTitle
                            textAlign="center"
                            subtitle="Timeline"
                            title="Working Process"
                            data-aos="fade-up"
                        />
                    </div>
                </div>
                <div class="row">
                    <div class="col-lg-10 offset-lg-1 mt--50">
                        <p>With years of expertise, we are the trusted digital marketers who employ proven strategies tailored to clients' needs and industry. Our focus on measurable results sets us apart, delivering unparalleled success.</p>
                        <Timeline :timeline-data="timelineData" :timeline-style="2"/>
                    </div>
                </div>
            </div>
        </div>
        <!-- End Timeline Area -->

        <Separator/>

        <!-- Start About Area -->
        <!-- <AboutTwo/> -->
        <!-- End About Area -->

        <TextArea1/>

        <Separator/>

        <!-- Start Pricing Area -->
        <!-- <div class="rwt-pricing-area rn-section-gap">
            <div class="container">
                <div class="row">
                    <div class="col-lg-12">
                        <SectionTitle
                            text-align="center"
                            subtitle="Take a Pricing"
                            title="Our Pricing Plan"
                            data-aos="fade-up"
                        />
                    </div>
                </div>
                <Pricing :pricing-data="pricingData" :pricing-style="5"/>
            </div>
        </div> -->
        <!-- End Pricing Area -->

        <!-- <Separator/> -->

        <!-- Start Brand Area -->
        <div class="rwt-brand-area rn-section-gap">
            <div class="container">
                <div class="row">
                    <div class="col-lg-12">
                        <SectionTitle
                            text-align="center"
                            subtitle="Our Awesome Client"
                            title="Trusted by the best clientele list with us"
                            data-aos="fade-up"
                        />
                    </div>
                </div>
                <div class="row">
                    <div class="col-lg-12 mt--40">
                        <Brand :brand-list="brandList"/>
                    </div>
                </div>
            </div>
        </div>
        <!-- End Brand Area  -->

        <div class="rwt-elements-area rn-section-gap">
            <div class="container">
                <div class="row mb--20">
                    <div class="col-lg-12">
                        <SectionTitle
                            text-align="center"
                            subtitle="Client Feedback"
                            title="Testimonial"
                            data-aos="fade-up"
                            data-aos-delay="60"
                        />
                    </div>
                </div>
                <Testimonial :testimonial="testimonialData"/>
            </div>
        </div>
    </Layout>
</template>

<script>
    import Layout from "../../components/common/Layout";
    import Separator from "../../components/elements/separator/Separator";
    import SectionTitle from "../../components/elements/sectionTitle/SectionTitle";
    import AboutTwo from "../../components/elements/about/AboutTwo";
    import Icon from "../../components/icon/Icon";
    import CallToAction from "../../components/elements/callToAction/CallToAction";
    import Timeline from "../../components/elements/timeline/Timeline";
    import Pricing from "../../components/elements/pricing/Pricing";
    import Brand from "../../components/elements/brand/Brand";
    import TextArea1 from "../../components/custom/textArea1";
    import Testimonial from "../../components/custom/testimonial";

    export default {
        name: 'SeoAgency',
        components: {Brand, Pricing, Timeline, CallToAction, Icon, AboutTwo, SectionTitle, Separator, Layout, TextArea1, Testimonial},
        data() {
            return {
                timelineData: [
                    {
                        id: '1',
                        title: 'Getting started',
                        description: 'Understand client business',
                    },
                    {
                        id: '2',
                        title: 'Planning',
                        description: 'Analyze Opportunities',
                    },
                    {
                        id: '3',
                        title: 'Execution',
                        description: 'Execute strategy',
                    },
                    {
                        id: '4',
                        title: 'Review',
                        description: 'Update progress report',
                    },
                ],
                pricingData: [
                    {
                        title: 'Basic Plan',
                        currency: '$',
                        price: '29',
                        subtitle: 'USD Per Month',
                        features: [
                            {title: '5 PPC Campaigns'},
                            {title: 'Digital Marketing'},
                            {title: 'Marketing Agency'},
                            {title: 'Seo Friendly'},
                            {title: 'UI/UX designs'},
                        ],
                        btn: {
                            text: 'Purchase Now',
                            link: '#'
                        }
                    },
                    {
                        title: 'Standard Plan',
                        currency: '$',
                        price: '50',
                        subtitle: 'USD Per Month',
                        features: [
                            {title: '5 PPC Campaigns'},
                            {title: 'Keep 100% Royalties'},
                            {title: 'App Development'},
                            {title: 'Seo Friendly'},
                            {title: 'UI/UX designs'},
                        ],
                        btn: {
                            text: 'Purchase Now',
                            link: '#'
                        },
                        isActive: true
                    },
                    {
                        title: 'Advanced Plan',
                        currency: '$',
                        price: '500',
                        subtitle: 'USD Per Month',
                        features: [
                            {title: '5 PPC Campaigns'},
                            {title: 'SEO Marketing'},
                            {title: 'Marketing Agency'},
                            {title: 'Seo Friendly'},
                            {title: 'Application Manage'},
                        ],
                        btn: {
                            text: 'Purchase Now',
                            link: '#'
                        }
                    }
                ],
                brandList: [
                    {
                        image: require(`@/assets/images/brand/brand-01.png`)
                    },
                    {
                        image: require(`@/assets/images/brand/brand-02.png`)
                    },
                    {
                        image: require(`@/assets/images/brand/brand-03.png`)
                    },
                    {
                        image: require(`@/assets/images/brand/brand-04.png`)
                    }
                ],
                testimonialData: [
                    {
                        description: 'Savvy Ray Tech has served as my marketing partner. I have admired some of the creative works that we received from them (both offline and online). They currently assist us in daily lead and inquiry generation on our website thanks to their SEO effectiveness. Good luck to the entire team!',
                        name: 'Mr Soni',
                        designation: 'Director of Silverspace Inc',
                        image: 'avatar-4.png'
                    },
                    {
                        description: 'From the beginning of our venture, Savvy Ray Technologies has been our partner. As a company, we have been working with them since inception, first for designing and developing our website, and then for all our online marketing needs. They have played an important role in the growth of our company by being extremely helpful & accommodating.',
                        name: 'Mr Pandya',
                        designation: 'Founder of Key Medsolutions',
                        image: 'avatar-3.png'
                    },
                    {
                        description: 'We were looking for a way to increase leads for our metal merchant business. We partnered with Savvy Ray Technologies  to create a Google Ads campaign that targeted our ideal customers. As a result, we saw a significant increase in leads, and we were able to close more sales. We are very pleased with the results and would highly recommend Savvy Ray Tech to other businesses.',
                        name: 'Sanjay Kumavat',
                        designation: 'Founder of SKD Aollys. Pvt ltd',
                        image: 'avatar-2.png'
                    },
                    {
                        description: 'I heartily endorse Savvy Ray Technologies for innovative design and brand awareness efforts. Their marketing team offers proactive advice and shares insightful strategies. Partnering with this company is beneficial, and they answer your requests immediately.',
                        name: 'Mr Dabhi',
                        designation: 'Co Founder of Vizva Consultancy Services (UK)',
                        image: 'avatar-1.png'
                    }
                ]
            }
        }
    }
</script>