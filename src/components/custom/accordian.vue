<template>
    <Layout>
        <!-- Start Accordion Area -->
        <div class="rn-accordion-area rn-section-gap pb--0 pt--0">
            <div class="container">
                <div class="row row--20">
                    <div class="col-lg-10 offset-lg-1">
                         <SectionTitle
                            text-align="center"
                            :subtitle="title"
                            data-aos="fade-up"
                            data-aos-delay="60"
                        />
                        <Accordion
                            accordion-style-class="rn-accordion-01"
                            :accordion-content="data"
                            data-aos="fade-up"
                            data-aos-delay="60"
                        />
                    </div>
                </div>
            </div>
        </div>
        <!-- End Accordion Area -->

    </Layout>
</template>

<script>
    import Accordion from '../elements/accordion/Accordion'
    import SectionTitle from '../elements/sectionTitle/SectionTitle'

    export default {
        name: 'homepageAccordian',
        components: {Accordion, SectionTitle},
        props: {
            data: {
                type: Array
            },
            title: {
                type: String
            }
        }
    }
</script>