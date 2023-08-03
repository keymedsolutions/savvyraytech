<template>
    <Layout>
        <!-- Start Accordion Area -->
        <div class="rn-accordion-area rn-section-gap pb--0">
            <div class="container">
                <!-- <div class="row">
                    <div class="col-lg-10 offset-lg-1">
                       
                    </div>
                </div> -->
                <div class="row row--20">
                    <div class="col-lg-10 offset-lg-1">
                         <SectionTitle
                            text-align="center"
                            subtitle="Get ready to experience jaw-dropping moments courtesy of our exceptional services"
                            title="The right audience will be waiting for you as well as the stage"
                            data-aos="fade-up"
                            data-aos-delay="60"
                        />
                        <Accordion
                            id="accordionExampleTwo"
                            accordion-style-class="rn-accordion-01"
                            :accordion-content="[
                                {
                                    id: 'one',
                                    title: 'Search Engine Optimization (SEO)',
                                    description: 'Helping your website become the leading player on Google. Our on-page and off-page optimizations elevate your presence across search engines.'
                                },
                                {
                                    id: 'two',
                                    title: 'Social Media Marketing (SSM)',
                                    description: 'Engage with your target customers and showcase your business across the dynamic landscape of social media. From Facebook and Instagram to Twitter, Pinterest, and LinkedIn, we ensure your presence on these platforms, allowing your audience to easily find and explore the offerings of your brand.'
                                },
                                {
                                    id: 'three',
                                    title: 'Pay Per Click (PPC) Marketing',
                                    description: 'Google Ads offers a comprehensive platform to engage with users across Google Search Engine and YouTube, enhancing your connectivity.'
                                },
                                {
                                    id: 'four',
                                    title: 'Design & Branding',
                                    description: 'While we certainly specialize in logo design, product packaging, and brand stationery, our true passion lies in infusing vitality into ideas, breathing life into brands.'
                                },
                                {
                                    id: 'five',
                                    title: 'Web Desgin & Development',
                                    description: `Our expertise lies in the creation and development of digital homes, better known as websites. Whether it's a fully bespoke website or a theme-based design using platforms like WordPress and Shopify, we have you covered.`
                                },
                                {
                                    id: 'six',
                                    title: 'Concept Shoots',
                                    description: 'We create captivating visuals for your brand, including campaigns, launches, and Instagram reels. Our team ensures lasting impressions and meaningful engagement. With our visual storytelling expertise, we elevate your online presence.'
                                },
                            ]"
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
        components: {Accordion, SectionTitle}
    }
</script>