<template>
    <ul class="mainmenu">
        <li><router-link to="/">Home</router-link></li>
            <!-- <ul class="submenu">
                <li><router-link to="/business-consulting">Business Consulting</router-link></li>
                <li><router-link to="/business-consulting-2">Business Consulting 02</router-link></li>
                <li><router-link to="/corporate">Corporate</router-link></li>
                <li><router-link to="/business">Business</router-link></li>
                <li><router-link to="/digital-agency">Digital Agency</router-link></li>
                <li><router-link to="/finance">Finance</router-link></li>
                <li><router-link to="/company">Company</router-link></li>
                <li><router-link to="/marketing-agency">Marketing Agency</router-link></li>
                <li><router-link to="/travel-agency">Travel Agency</router-link></li>
                <li><router-link to="/consulting">Consulting</router-link></li>
                <li><router-link to="/seo-agency">SEO Agency</router-link></li>
                <li><router-link to="/personal-portfolio">Personal Portfolio</router-link></li>
                <li><router-link to="/event-conference">Event Conference</router-link></li>
                <li><router-link to="/creative-portfolio">Creative Portfolio</router-link></li>
                <li><router-link to="/freelancer">Freelancer</router-link></li>
                <li><router-link to="/international-consulting">International Consulting</router-link></li>
                <li><router-link to="/startup">Startup</router-link></li>
                <li><router-link to="/web-agency">Web Agency</router-link></li>
            </ul> -->
        <li class="has-droupdown has-menu-child-item">
            <a href="#">
                What we do
                <Icon name="plus" class="collapse-icon plus"/>
                <Icon name="minus" class="collapse-icon minus"/>
            </a>
            <ul class="submenu">
                <li><router-link to="/search-engine-optimization">Search Engine Optimization</router-link></li>
                <li><router-link to="/social-media-marketing">Social Media Marketing</router-link></li>
                <li><router-link to="/pay-per-click">Pay per click</router-link></li>
                <li><router-link to="/web-design-development">Web Desgin & Development</router-link></li>
                <li><router-link to="/concept-shoots">Concept Shoots</router-link></li>
                <li><router-link to="/branding">Branding</router-link></li>
            </ul>
        </li>
        <li><router-link to="/about-us">About us</router-link></li>
        <!-- <li><router-link to="/careers"> Careers - Life at Savvy Ray</router-link></li>
        <li><router-link to="/blog">Blog</router-link></li> -->
        <li><router-link to="/contact-us">Contact Us</router-link></li>
        <!-- <li class="with-megamenu has-menu-child-item">
            <a href="#">
                Elements
                <Icon name="plus" class="collapse-icon plus"/>
                <Icon name="minus" class="collapse-icon minus"/>
            </a>
            <div class="rn-megamenu">
                <div class="wrapper">
                    <div class="row row--0">
                        <div class="col-lg-3 single-mega-item">
                            <ul class="mega-menu-item">
                                <li><router-link to="/button">Button</router-link></li>
                                <li><router-link to="/service">Service</router-link></li>
                                <li><router-link to="/counter">Counter</router-link></li>
                                <li><router-link to="/progressbar">Progressbar</router-link></li>
                                <li><router-link to="/accordion">Accordion</router-link></li>
                                <li><router-link to="/social-share">Social Share</router-link></li>
                                <li><router-link to="/blog-grid">Blog Grid</router-link></li>
                            </ul>
                        </div>
                        <div class="col-lg-3 single-mega-item">
                            <ul class="mega-menu-item">
                                <li><router-link to="/team">Team</router-link></li>
                                <li><router-link to="/portfolio">Portfolio</router-link></li>
                                <li><router-link to="/testimonial">Testimonial</router-link></li>
                                <li><router-link to="/timeline">Timeline</router-link></li>
                                <li><router-link to="/tab">Tab</router-link></li>
                                <li><router-link to="/pricing">Pricing</router-link></li>
                                <li><router-link to="/spit-section">Split Section</router-link></li>
                            </ul>
                        </div>
                        <div class="col-lg-3 single-mega-item">
                            <ul class="mega-menu-item">
                                <li><router-link to="/call-to-action">Call To Action</router-link></li>
                                <li><router-link to="/video">Video</router-link></li>
                                <li><router-link to="/gallery">Gallery</router-link></li>
                                <li><router-link to="/contact">Contact</router-link></li>
                                <li><router-link to="/brand">Brand</router-link></li>
                                <li><router-link to="/portfolio">Portfolio</router-link></li>
                                <li><router-link to="/error">404</router-link></li>
                            </ul>
                        </div>
                        <div class="col-lg-3 single-mega-item">
                            <ul class="mega-menu-item">
                                <li>
                                    <router-link to="/advance-tab">
                                        Advance Tab <span class="rn-badge-card">Hot</span>
                                    </router-link>
                                </li>
                                <li>
                                    <router-link to="#">
                                        Brand Carousel <span class="rn-badge-card">Comming</span>
                                    </router-link>
                                </li>
                                <li>
                                    <router-link to="/advance-pricing">
                                        Advance Pricing <span class="rn-badge-card">Hot</span>
                                    </router-link>
                                </li>
                                <li>
                                    <router-link to="/portfolio-details/1">
                                        Portfolio Details
                                    </router-link>
                                </li>
                                <li>
                                    <router-link to="/blog-details/1">
                                        Blog Details
                                    </router-link>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </li>
        <li class="has-droupdown has-menu-child-item">
            <a href="#">
                Blog
                <Icon name="plus" class="collapse-icon plus"/>
                <Icon name="minus" class="collapse-icon minus"/>
            </a>
            <ul class="submenu">
                <li><router-link to="/blog-grid">Blog Grid</router-link></li>
                <li><router-link to="/blog-grid-sidebar">Blog Grid Sidebar</router-link></li>
                <li><router-link to="/blog-list">Blog List View</router-link></li>
                <li><router-link to="/blog-list-sidebar">Blog List View Sidebar</router-link></li>
            </ul>
        </li>
        <li class="has-droupdown has-menu-child-item">
            <a href="#">
                Portfolio
                <Icon name="plus" class="collapse-icon plus"/>
                <Icon name="minus" class="collapse-icon minus"/>
            </a>
            <ul class="submenu">
                <li><router-link to="/portfolio">Portfolio Default</router-link></li>
                <li><router-link to="/portfolio-three-column">Portfolio Three Column</router-link></li>
                <li><router-link to="/portfolio-full-width">Portfolio Full Width</router-link></li>
                <li><router-link to="/portfolio-grid-layout">Portfolio Grid Layout</router-link></li>
                <li><router-link to="/portfolio-box-layout">Portfolio Box Layout</router-link></li>
            </ul>
        </li>
        <li><router-link to="/contact">Contact</router-link></li> -->
    </ul>
</template>

<script>
    import Icon from "../../icon/Icon";
    export default {
        name: 'Nav',
        components: {Icon}
    }
</script>