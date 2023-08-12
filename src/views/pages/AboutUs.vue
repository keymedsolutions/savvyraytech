<template>
    <Layout header-class="header-transparent" :show-cta="false">
        <!-- Start Slider Area -->
        <div class="slider-area slider-style-1 height-850 bg_image"
             data-black-overlay="7"
             :style="{'background-image': `url(${require(`@/assets/images/bg/12.jpg`)})`}">
            <div class="container">
                <div class="row">
                    <div class="col-lg-12">
                        <div class="inner pt--80 text-center">
                            <div>
                                <h3 class="rn-sub-badge" data-aos="fade-up" data-aos-delay="100">
                                    <span class="theme-gradient">Our Company's Details.</span>
                                </h3>
                            </div>
                            <h1 class="title display-one" data-aos="fade-up" data-aos-delay="150">
                                Thank you for allowing us to introduce ourselves and highlight our expertise.
                            </h1>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- End Slider Area -->

        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="inner pt--80 text-center">
                            <h3 class="rn-sub-badge" data-aos="fade-up" data-aos-delay="100">
                                <span class="theme-gradient">Let us brief you</span>
                            </h3>
                    </div>
                </div>
            </div>
        </div>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="briefData1"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="briefData2"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="briefData3"/>        
        <Separator/>

        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="inner pt--80 text-center">
                            <h3 class="rn-sub-badge" data-aos="fade-up" data-aos-delay="100">
                                <span class="theme-gradient">Our vision</span>
                            </h3>
                    </div>
                </div>
            </div>
        </div>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="vision"/>      
        <Separator/>
        
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="inner pt--80 text-center">
                            <h3 class="rn-sub-badge" data-aos="fade-up" data-aos-delay="100">
                                <span class="theme-gradient">Our mission</span>
                            </h3>
                    </div>
                </div>
            </div>
        </div>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="mission"/>      
       
    </Layout>
</template>

<script>
    import Layout from '@/components/common/Layout'
    import Separator from '@/components/elements/separator/Separator'
    import TextComponent from '@/components/custom/textComponent'

    export default {
        name: 'About',
        components: {Separator, Layout, TextComponent},
        data() {
            return {
                briefData1: {
                    description: `Savvy Ray Technologies is a proficient Digital Marketing agency located in Ahmedabad and the US. We specialize in providing comprehensive 360° Digital Solutions, encompassing Search Engine Optimization (SEO), Web design, Web Development, Social Media Optimization and Management (SMO/SMM), Concept photos and Video shoots, and Graphic design. With a team of skilled professionals experienced in managing digital channels, our aim is to elevate your business to the forefront of search engine rankings.`
                },
                briefData2: {
                    description: `As we enhance your digital presence, boost sales, generate business leads, and optimize IT, we maximize your return on investment (ROI). Our approach is driven by performance-focused strategies, leveraging advanced technological capabilities, and utilizing our expertise in digital marketing. The digital marketing services we offer cater to industries such as pharmaceuticals, healthcare, real estate, IT, e-commerce, manufacturing, education, brands, and FMCG.`
                },
                briefData3: {
                    description: `At Savvy Ray Technologies, we are dedicated to delivering exceptional results and empowering our clients to thrive in the ever-evolving digital landscape.`
                },
                vision: {
                    description: `To become the leading integrated digital marketing partner in Ahmedabad and the US, relentlessly pursuing accelerated and sustainable growth for brands worldwide.`
                },
                mission: {
                    description: 'A team of marketing professionals that has a deep understanding of digital marketing nuances is built by leveraging conventional and unconventional strategies and tactics.'
                }
            }
        }
    }
</script>