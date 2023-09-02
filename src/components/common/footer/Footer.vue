<template>
    <div>
        <!-- Start Footer Area  -->
        <footer v-if="data.showFooter" class="rn-footer footer-style-default variation-two">
            <div v-if="data.showCta" class="rn-callto-action clltoaction-style-default style-7">
                <div class="container">
                    <div class="row row--0 align-items-center content-wrapper font-16">
                        <SectionTitle
                            textAlign="left"
                            title=""
                            subtitle="Outperform your competition"
                            data-aos="fade-up"
                        />
                        <div class="col-lg-8 col-md-8">
                            <div class="inner" data-aos="fade-up">
                                <div class="content text-left">
                                    
                                    <p class="mb--0">
                                        Partner with us for remarkable success in brand awareness, customer engagement, and revenue generation. Let's connect and stay ahead in your industry.
                                    </p>
                                </div>
                            </div>
                        </div>
                        <div class="col-lg-4 col-md-4">
                            <div class="call-to-btn text-start mt_sm--20 text-lg-end" data-aos="fade-up">
                                <Button
                                    title="Let’s Talk"
                                    icon="arrow-right"
                                    url="/contact-us"
                                />
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="footer-top pb-0">
                <div class="container">
                    <div class="row">
                        <div class="col-lg-2 col-md-6 col-sm-6 col-12">
                            <div class="rn-footer-widget">
                                <h4 class="title">Details</h4>
                                <div class="inner">
                                    
                                    <h4 class="subtitle mb-3 mt-3">Address: </h4>
                                    <span>Greensboro, North Carolina, USA</span>
                                </div>
                            </div>
                        </div>
                        <div class="col-lg-5 col-md-6 col-sm-6 col-12">
                            <div class="rn-footer-widget">
                                <div class="widget-menu-top">
                                    <h4 class="title"> What we do</h4>
                                    <div class="inner">
                                        <div class="row">
                                            <div class="col-lg-6">
                                                <ul class="footer-link link-hover">
                                            <li>
                                                <router-link to="/digital-marketing">Digital Marketing</router-link>
                                            </li>
                                            <li>
                                                <router-link to="/search-engine-optimization">Search Engine Optimization</router-link>
                                            </li>
                                            <li>
                                                <router-link to="/social-media-marketing">Social Media Marketing</router-link>
                                            </li>
                                           
                                        </ul>
                                            </div>
                                            <div class="col-lg-6">
                                        <ul class="footer-link link-hover">
                                            <li>
                                                <router-link to="/search-engine-marketing">Search Engine Marketing</router-link>
                                            </li>
                                            <li>
                                                <router-link to="/web-design-development">Web Desgin & Development</router-link>
                                            </li>
                                            <li>
                                                <router-link to="/concept-shoots">Concept Shoots</router-link>
                                            </li>
                                        </ul>
                                            </div>
                                        </div>
                                        
                                    </div>
                                </div>
                            </div>
                        </div>
                        <!-- <div class="col-lg-2 col-md-6 col-sm-6 col-12">
                            <div class="rn-footer-widget">
                                <h4 class="title">Company</h4>
                                <div class="inner">
                                    <ul class="footer-link link-hover">
                                        <li>
                                            <router-link to="/pricing">Pricing</router-link>
                                        </li>
                                        <li>
                                            <router-link to="/tab">Tab Styles</router-link>
                                        </li>
                                        <li>
                                            <router-link to="/service">Service</router-link>
                                        </li>
                                        <li>
                                            <router-link to="/social-share">Social</router-link>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </div> -->
                        <div class="col-lg-3 col-md-6 col-sm-6 col-12">
                            <div class="rn-footer-widget">
                                <h4 class="title">Other links</h4>
                                <div class="inner">
                                    <ul class="footer-link link-hover">
                                        <!-- <li>
                                            <router-link to="/careers">Careers</router-link>
                                        </li> -->
                                        <li>
                                            Email: <a href="mailto:info@savvyraytech.com">info@savvyraytech.com</a>
                                        </li>
                                        <li>
                                            Telephone: <a href="tel:+13366957819"> +1 336-695-7819</a>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                        <div class="col-lg-2 col-md-6 col-sm-6 col-12">
                            <div class="rn-footer-widget">
                                <h4 class="title">Stay connected</h4>
                                <div class="inner">
                                    <Logo/>
                                    <!-- <h6 class="subtitle">2000+ Our clients are subscribe Around the World</h6> -->
                                    
                                    <!-- <ul class="footer-link link-hover">
                                        <li>
                                            <router-link to="/careers">Careers</router-link>
                                        </li>
                                        <li>
                                            Email: <a href=":mailto=user@email.com">user@email.com</a>
                                        </li>
                                        <li>
                                            HR: <router-link to="/careers">HR</router-link>
                                        </li>
                                    </ul> -->
                                    <ul class="social-icon social-default justify-content-start mt--5">
                                        <li>
                                            <a href="https://www.facebook.com/savvyraytechnologies/" target="_blank">
                                                <Icon name="facebook"/>
                                            </a>
                                        </li>
                                        <li>
                                            <a href="https://www.instagram.com/savvyraytechnologies/" target="_blank">
                                                <Icon name="instagram"/>
                                            </a>
                                        </li>
                                        <li>
                                            <a href="https://www.linkedin.com/company/savvy-ray-technologies/" target="_blank">
                                                <Icon name="linkedin"/>
                                            </a>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <Newsletter v-if="data.showNewsletter"/>
        </footer>
        <!-- End Footer Area  -->

        <Copyright v-if="data.showCopyright"/>

        <ScrollTop/>
    </div>
</template>

<script>
    import Copyright from './Copyright'
    import Button from '../../elements/button/Button'
    import Icon from '../../icon/Icon'
    import ScrollTop from './ScrollTop'
    import Logo from '../../elements/logo/Logo'
    import Newsletter from './Newsletter'
    import SectionTitle from "../../elements/sectionTitle/SectionTitle";

    export default {
        name: 'Footer',
        components: {Newsletter, Logo, ScrollTop, Icon, Button, Copyright, SectionTitle},
        props: {
            data: {
                default: null
            }
        }
    }
</script>