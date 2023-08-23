<template>
     <Layout header-class="header-transparent" buy-button-class="btn-default btn-small">
        <Breadcrumb :current-url="name" :title="name"/>
         <SectionTitle
            class="mt--30"
            text-align="center"
            subtitle="Concept photo & video shoots in Ahmedabad"
            data-aos="fade-up"
            data-aos-delay="60"
        />
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="csData.para1" :noDescriptionMargin="true"/>
        <Separator />
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="csData.para2" :noDescriptionMargin="true"/>
        <Separator />
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="csData.para3" :noDescriptionMargin="true"/>
        <Separator />
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="csData.para4" :noDescriptionMargin="true"/>
        <Separator />
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="csData.para5" :noDescriptionMargin="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="csData.para6" :noDescriptionMargin="true"/>
        <Separator />
        <div class="container pt--60 pb--60">
            <div class="row">
                <Accordian :title="csData.accordianData1.title" :data="csData.accordianData1.data" />
            </div>
        </div>
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
    name: 'ConceptShoots',
        components: {Layout, Breadcrumb, TextComponent, Separator, SectionTitle, Accordian },

    data() {
        return {
            name: 'Concept shoots',
            csData: {
                para1: {
                    title: `Unleash the Power of Visual Storytelling!`,
                    description: `In today's visually driven world, captivating imagery and videos are essential for generating interest and desire for your products or services. At Flora Fountain, we specialize in professionally planned and executed photo and video shoots in Ahmedabad. With our expertise in lifestyle, jewelry, and F&B brands, we transform ordinary visuals into extraordinary experiences.`
                },
                para2: {
                    title: `Creating Unique Concepts for Your Brand`,
                    description: `We understand that creating a concept is a delicate blend of creativity, psychology, and brand ideology. By studying your brand's vision and consumer behavior, we craft concepts that resonate and delight your target audience. Step into their shoes, reimagine their thought process, and spark a new desire for your offerings.`
                },
                para3: {
                    title: `Mastering the Art of Direction`,
                    description: `Art direction is our forte. We believe every frame should convey a powerful message through meticulous attention to detail. From color selection to product placement, we ensure every element enhances your brand's visual appeal. We leave no stone unturned in capturing the essence of your brand.`
                },
                para4: {
                    title: `Seamless Shoot Planning and Execution`,
                    description: `Managing a shoot involves more than just capturing photos or videos. We take care of the entire process, from location scouting to connecting you with talented professionals in Ahmedabad. With our hands-on approach, we personally oversee every aspect of the shoot, ensuring a seamless and successful outcome.`
                },
                para5: {
                    title: `Diverse Shoots Tailored to Your Needs`,
                    description: `Whether you require an e-commerce shoot, product photography, or social media content creation, we've got you covered. Our specially curated shoots cater to your unique requirements, ensuring your brand stands out on various platforms. From static posts to animated stories, we bring your brand to life.`
                },
                para6: {
                    description: `Unleash the visual allure of your brand with our exceptional concepts and captivating imagery. Together, let's create visual treats that leave a lasting impression on your consumers!`
                },
                accordianData1: {
                    title: 'Our Expertise in Various Shoots:',
                    data: [
                        {
                            id: 'One',
                            title: 'E-Commerce Shoot',
                            description: `We specialize in creating exceptional photography and videography specifically tailored for your e-commerce website and online shop. With our carefully curated visuals, we aim to enhance your products' appeal and drive conversions.`
                        },
                        {
                            id: 'Two',
                            title: 'Product Photography',
                            description: "Our expertise extends to product photography, where we focus solely on capturing the essence of your products. From delectable treats like cookies to stylish clothing items and even robust beverages like tea, we showcase your offerings in their best light."
                        },
                        {
                            id: 'Three',
                            title: 'Shoot for Social Media',
                            description: `Engage and captivate your audience on social media with our expertly crafted photographs and videos. We create content exclusively designed for your brand's social media presence, including static posts, animated stories, attention-grabbing GIFs, IGTV videos, and captivating reels.`
                        },
                        {
                            id: 'Four',
                            title: 'Delight Your Consumers with Visual Treats',
                            description: `With our unique concepts and meticulous attention to detail, we strive to create visual treats that leave a lasting impression on your consumers. By combining our creativity and your brand's essence, we craft compelling visuals that resonate with your target audience.`
                        }
                    ]
                }
            }
        }
    }
}
</script>