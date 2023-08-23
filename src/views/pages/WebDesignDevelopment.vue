<template>
     <Layout header-class="header-transparent" buy-button-class="btn-default btn-small">
        <Breadcrumb :current-url="name" :title="name"/>
        <SectionTitle
            class="mt--30"
            text-align="center"
            subtitle="Transforming websites into masterpieces"
            data-aos="fade-up"
            data-aos-delay="60"
        />
         <TextComponent data-aos="fade-up" data-aos-delay="100" :data="wddData.para1" :noDescriptionMargin="true"/>
         <TextComponent data-aos="fade-up" data-aos-delay="100" :data="wddData.para2" :noDescriptionMargin="true"/>
         <TextComponent data-aos="fade-up" data-aos-delay="100" :data="wddData.para3" :noDescriptionMargin="true"/>
         <TextComponent data-aos="fade-up" data-aos-delay="100" :data="wddData.para4" :noDescriptionMargin="true"/>
        <Separator />
        <div class="container pt--60 pb--60">
            <div class="row">
                <Accordian :title="accordianData1.title" :data="accordianData1.data" />
            </div>
        </div>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="wddData.para5" :noDescriptionMargin="true"/>
        <Separator />
        <!-- <div class="container pt--60 pb--60">
            <div class="row">
                <Accordian :title="accordianData2.title" :data="accordianData2.data" />
            </div>
        </div>
        <Separator />
        <div class="container pt--60 pb--60">
            <div class="row">
                <Accordian :title="accordianData3.title" :data="accordianData3.data" />
            </div>
        </div>
        <Separator /> -->
        <div class="container mb--60 mt--60">
            <div class="row">
                <div class="col-md-6">
                    <Accordian :title="accordianData2.title" :data="accordianData2.data" />
                </div>
                <div class="col-md-6">
                    <Accordian :title="accordianData3.title" :data="accordianData3.data" />
                </div>
            </div>
        </div>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="wddData.para6" :noDescriptionMargin="true"/>
    </Layout>
</template>
<script>
import Breadcrumb from '@/components/elements/breadcrumb/Breadcrumb.vue';
import Layout from "../../components/common/Layout";
import TextComponent from '@/components/custom/textComponent.vue';
import Separator from '@/components/elements/separator/Separator'
import SectionTitle from '@/components/elements/sectionTitle/SectionTitle';
import Accordian from '@/components/custom/accordian.vue';

export default {
    name: 'WebDesignDevelopment',
    components: {Layout, Breadcrumb, TextComponent, Separator, SectionTitle, Accordian },

    data() {
        return {
            name: 'Web design and development',
            wddData: {
                para1: {
                    title: `Cost-effective, customer-centric, and ready for success!`,
                    description: `Don't settle for a pretty website with missing information and a confusing user experience. At Savvy Ray Technologies, we ensure your website is a seamless blend of aesthetics and usability.`
                },
                para2: {
                    description: `Our expert team of web designers crafts websites that showcase your brand's personality while prioritizing user experience. We understand that brands seek web development to create a lasting impact, and that's exactly what we deliver.`
                },
                para3: {
                    description: `With a focus on customization, our top-notch website developers build your website from scratch, incorporating the right aesthetics, functionality, and appeal. We emphasize speed, smoothness, and security, ensuring your website is optimized for mobile devices.`,
                },
                para4: {
                    description: `A website should leave a lasting impression through an exceptional user experience, and our services align with the expertise of any leading UX design agency in the US and India. Are you ready for an exciting journey of creative construction? Let's get started!`
                },
                para5: {
                    description: `When you choose Savvy Ray Technologies, you're partnering with a web design and development company that is committed to delivering exceptional results. We bring your digital vision to life, creating a website that not only looks stunning but also drives meaningful connections and experiences with your audience.`
                },
                para6: {
                    description: `Choose our web development services to build a website that aligns with your goals and engages your target audience effectively. Let us transform your vision into a functional and visually appealing digital platform.`
                },
            },
            accordianData1: {
                title: `What sets us apart at Savvy Ray Technologies? Here's why you should choose us:`,
                data: [
                    {
                        id: 'wdd1-1',
                        title: 'Unforgettable First Impressions',
                        description: `We understand that your website is the face of your brand online. Within seconds, it needs to capture visitors' attention and make a lasting impression. Our designs are visually striking and user-friendly, ensuring a positive and engaging experience from the moment users land on your site.`
                    },
                    {
                        id: 'wdd1-2',
                        title: 'Customer-Centered Approach',
                        description: `We put your customers first. Our websites are built with their needs and preferences in mind. We carefully craft the user experience, making it intuitive and seamless, so visitors can easily find the information they're looking for and take the desired actions.`
                    },
                    {
                        id: 'wdd1-3',
                        title: 'Functionality and Performance',
                        description: `Our focus extends beyond aesthetics. We prioritize functionality and performance to ensure your website works flawlessly. We optimize for speed, security, and responsiveness across all devices, providing a smooth browsing experience that keeps visitors engaged.`
                    },
                    {
                        id: 'wdd1-4',
                        title: 'Enriching User Lives',
                        description: `We believe in the transformative power of your products or services. Our web design and development services aim to enhance the lives of your users. We create intuitive interfaces and seamless interactions, making their digital journey easier, more enjoyable, and ultimately more impactful.`
                    }
                ]
            },
            accordianData2: {
                title: `At Savvy Ray Technologies, we take pride in nurturing your brand through our web development services`,
                data: [
                    {
                        id: 'wdd2-1',
                        title: 'Custom Website Development',
                        description: `We specialize in building tailor-made websites that are unique to your brand. Our custom web development solutions ensure that your website stands out and leaves a lasting impression on your audience.`
                    },
                    {
                        id: 'wdd2-2',
                        title: 'Mobile Sites',
                        description: `We create mobile websites that are fully optimized for smart devices. With our expertise, your website will deliver a seamless and engaging experience across various mobile platforms.`
                    },
                    {
                        id: 'wdd2-3',
                        title: 'Responsive Website Development',
                        description: `Our skilled web developers craft responsive websites that adapt to different screen sizes and devices. This ensures that your website looks great and functions flawlessly on any browser or device, enhancing user satisfaction and driving business growth.`
                    },
                    {
                        id: 'wdd2-4',
                        title: 'CMS Development',
                        description: `We offer CMS (Content Management System) development services, enabling you to easily manage and update your website's content. Our team can work with your preferred CMS platform, ensuring speed, SEO-friendliness, and customized features.`
                    },
                    {
                        id: 'wdd2-5',
                        title: 'Front-end Development',
                        description: `Our front-end developers create visually appealing and user-friendly interfaces for websites and web applications. We focus on delivering a seamless user experience that captivates your visitors and encourages interaction.`
                    },
                    {
                        id: 'wdd2-6',
                        title: 'Backend  Development',
                        description: `Our experienced backend developers handle the technical aspects of your website, including database design, backend coding, API integration, business logic implementation, and server management. We ensure a robust and reliable foundation for your website's functionality.`
                    },
                    {
                        id: 'wdd2-7',
                        title: 'Full-stack Development',
                        description: `With our full-stack developers, you can rely on comprehensive expertise in both front-end and back-end development. From gathering requirements to testing and deployment, our team can handle the entire development process with efficiency and precision.`
                    },
                    {
                        id: 'wdd2-8',
                        title: 'API Integration',
                        description: `We understand the importance of API integration for modern applications and portals. Our experts can seamlessly integrate and develop APIs to enhance the functionality and authentication of your website.`
                    },
                ]
            },
            accordianData3: {
                title: `At our web development agency, we specialize in building a variety of websites to cater to your specific needs:`,
                data: [
                    {
                        id: 'wdd3-1',
                        title: 'Corporate Websites',
                        description: `We create professional corporate websites that instill trust and showcase your brand to potential customers. Present your company with confidence and make a lasting impression.`
                    },
                    {
                        id: 'wdd3-2',
                        title: 'Web Portals',
                        description: `We can turn any custom web portal concept into reality, whether it's for web apps, travel, matrimony, e-commerce, or other innovative ideas. We bring your portal vision to life.`
                    },
                    {
                        id: 'wdd3-3',
                        title: 'B2B Websites',
                        description: `Connect with other businesses and expand your online presence with our B2B and B2C website design and development services. Strengthen your business relationships and drive growth.`
                    },
                    {
                        id: 'wdd3-4',
                        title: 'CMS Websites',
                        description: `Our expertise lies in developing CMS websites that store content in a database and present it dynamically using templates. Enjoy the flexibility of managing and updating your website effortlessly.`
                    },
                    {
                        id: 'wdd3-5',
                        title: 'Personal Websites',
                        description: `Stand out from the crowd with a unique personal website that promotes your career, allows you to connect with others, or serves as a platform for self-expression. Let your online presence reflect your individuality.`
                    },
                    {
                        id: 'wdd3-6',
                        title: 'Blog Websites',
                        description: `Keep your audience engaged with our dynamic blog websites, regularly updated with fresh and valuable content. Share your knowledge, insights, and expertise in an appealing and organized format.`
                    },
                    {
                        id: 'wdd3-7',
                        title: 'WordPress Websites',
                        description: `Our skilled custom WordPress developers create user-friendly websites that incorporate CMS functionality and are optimized for conversions. Leverage the power of WordPress for your business growth.`
                    },
                    {
                        id: 'wdd3-8',
                        title: 'Lead Generation Websites',
                        description: `Generate quality leads with our lead generation websites that capture user information and go beyond a simple digital brochure. Educate your audience and nurture potential customers.`
                    },
                    {
                        id: 'wdd3-9',
                        title: 'Business Websites',
                        description: `Effectively communicate vital information about your business, products, and services through our well-crafted business websites. Showcase your offerings and establish your online presence.`
                    },
                ]
            }
        }
    }
}
</script>