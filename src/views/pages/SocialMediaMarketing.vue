<template>
     <Layout header-class="header-transparent" buy-button-class="btn-default btn-small">
        <Breadcrumb :current-url="name" :title="name"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="smmData.para1" :noDescriptionMargin="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="smmData.para2" :noDescriptionMargin="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="smmData.para3" :noDescriptionMargin="true"/>
        <Separator />
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="smmData.para4" :noDescriptionMargin="true"/>
        <Flow :serviceList="serviceList"/>
        <Separator />
        <SectionTitle
            class="mt--30"
            text-align="center"
            subtitle="We Empower Your Social Media Journey To:"
            data-aos="fade-up"
            data-aos-delay="60"
        />
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="smmData.list1" :showList="true"/>
        <Separator />

        <section class="rn-service-area rn-section-gap">
            <div class="container">
                <div class="row row--30">
                    <div class="col-lg-12">
                        <SectionTitle
                            class="mb--30"
                            text-align="center"
                            subtitle='We Provide Well Planned Social Media Marketing Services For Industries'
                            title="Our SMM Services"
                            data-aos="fade-up"
                            data-aos-delay="60"
                        />
                    </div>
                </div>
                <Cards :serviceList="serviceList2"/>
            </div>
        </section>
    </Layout>
</template>
<script>
import Breadcrumb from '@/components/elements/breadcrumb/Breadcrumb.vue';
import Layout from "../../components/common/Layout";
import TextComponent from '@/components/custom/textComponent.vue';
import Flow from '@/components/custom/flow.vue';
import Separator from '@/components/elements/separator/Separator';
import SectionTitle from '@/components/elements/sectionTitle/SectionTitle';
import Cards from '@/components/custom/cards.vue';

export default {
    name: 'SocialMediaMarketing',
        components: {Layout, Breadcrumb, TextComponent, Separator, SectionTitle, Flow, Cards},

    data() {
        return {
            name: 'Social media marketing',
            smmData: {
                para1: {
                    title: 'Social Media Agency & Branding',
                    description: `Say goodbye to old-school marketing tactics! In today's digital era, social media has transformed the way businesses reach their audience. At Savvy Ray Technologies, we specialize in creating compelling social media strategies that drive business growth. As the leading social media marketing company in Ahmedabad, we focus on branding and delivering measurable results.`
                },
                para2: {
                    description: "Our team of experts takes the time to understand your brand, business goals, and online presence. With our tailored approach, we optimize your return on investment by creating engaging social media interactions that resonate with your target audience. From captivating content to eye-catching visuals, we know how to make your brand shine on social media."
                },
                para3: {
                    description: "In addition to our social media expertise, we offer comprehensive digital marketing services, including video production and management. Let us simplify the world of social media for you and help you elevate your digital marketing efforts. Get ready to make a lasting impact with Savvy Ray Technologies! Contact us today to get started."
                },
                para4: {
                    title: `Looking to boost your online sales?`,
                    description: `Put an end to your social media struggles. Partner with the leading SMO agency Savvy Ray Technologies and unlock the power of social media management services. Our expert team will optimize your brand's reach, foster customer loyalty, and drive sales. Level up your online sales with our professional expertise. Contact us today for outstanding results.`
                },
                para5: {
                    title: 'We Provide Well Planned Social Media Marketing Services For Industries'
                },
                list1: {
                    list: [
                        '● Connect effortlessly with your target audience.',
                        "● Establish trust and foster a positive brand identity.Engage followers and build brand loyalty.",
                        "● Foster meaningful conversations with potential customers.",
                        "● Identify the perfect social platforms for your business.",
                        "● Create a growth plan backed by thorough research.",
                        "● Cultivate an authentic community of dedicated followers.",
                        "● Craft and schedule compelling posts, tweets, and pins.",
                        "● Develop impactful ads and sponsored content.",
                        "● Promote your latest news, events, and products.",
                        "● Enhance brand loyalty and surpass competitors.",
                        "● Elevate your brand image and reputation."
                    ],
                }
            },
            serviceList: [
                {
                    icon: '1',
                    title: 'SMM Consultation',
                    description: 'Expand your customer base with a strategic blend of organic and paid social media marketing techniques.'
                },
                {
                    icon: '2',
                    title: 'SMM Strategy',
                    description: "Crafting distinctive and effective strategies to maximize your brand's impact on social media platforms."
                },
                {
                    icon: '3',
                    title: "SMM Calendar",
                    description: "Streamline and accelerate your marketing efforts with our content calendar. Plan. Schedule. Boost productivity and business efficiency."
                },
                {
                    icon: '4',
                    title: "SMM Management ",
                    description: "Experience comprehensive services and personalized management to elevate your brand and drive business growth."
                }
            ],
            serviceList2: [
                { title: 'Small business' },
                { title: 'Startups' },
                { title: 'Company' },
                { title: 'Outlets' },
                { title: 'Brands' },
                { title: 'Ecommerce' },
                { title: 'Celebrities' },
                { title: 'Apparel' },
                { title: 'Restaurants' },
                { title: 'Hotels' },
            ],
        }
    }
}
</script>