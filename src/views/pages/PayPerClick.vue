<template>
     <Layout header-class="header-transparent" buy-button-class="btn-default btn-small">
        <Breadcrumb :current-url="name" :title="name"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para1" :noDescriptionMargin="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para2" :noDescriptionMargin="true" :showList="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para3" :noDescriptionMargin="true"/>
        <Separator />
       
        <SectionTitle
            class="mt--30"
            text-align="center"
            subtitle="We initiate the Keyword Research process for your website"
            data-aos="fade-up"
            data-aos-delay="60"
        />
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para4" :noDescriptionMargin="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para5" :noDescriptionMargin="true"/>
       
        <Separator />
        
        <SectionTitle
            class="mt--30"
            text-align="center"
            subtitle="Building your comprehensive Keyword list"
            data-aos="fade-up"
            data-aos-delay="60"
        />
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para6" :noDescriptionMargin="true"/>

        <Separator />

        <SectionTitle
            class="mt--30"
            text-align="center"
            subtitle="The Google AdWords Process"
            data-aos="fade-up"
            data-aos-delay="60"
        />
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para7" :noDescriptionMargin="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para8" :noDescriptionMargin="true" :showList="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para9" :noDescriptionMargin="true"/>

        <Separator />
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para10" :noDescriptionMargin="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para11" :noDescriptionMargin="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para12" :noDescriptionMargin="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="semData.para13" :noDescriptionMargin="true"/>
    </Layout>
</template>
<script>
import Breadcrumb from '@/components/elements/breadcrumb/Breadcrumb.vue';
import Layout from "../../components/common/Layout";
import TextComponent from '@/components/custom/textComponent.vue';
import Separator from '@/components/elements/separator/Separator'
import SectionTitle from '@/components/elements/sectionTitle/SectionTitle';

export default {
    name: 'PayPerClick',
        components: {Layout, Breadcrumb, TextComponent, Separator, SectionTitle},

    data() {
        return {
            name: 'Pay per click',
            semData: {
                para1: {
                    title: 'Google Adwords',
                    description: `Choosing the right keywords is vital for a successful AdWords campaign. It's all about increasing visibility by targeting the keywords your potential customers use when searching. Your keyword strategy is key to campaign effectiveness. To conduct effective keyword research, put yourself in your audience's shoes.`
                },
                para2: {
                    description: `Ask yourself:`,
                    list: [
                        '● What keywords do people use to find my product?',
                        '● How can people engage with my blog?',
                    ]
                },
                para3: {
                    description: `Answering these questions provides valuable insights and helps you select relevant keywords to enhance your AdWords campaign.`
                },
                para4: {
                    description: `Using Google tools like Google Search Console and Google Analytics, we thoroughly analyze your website to gain insights into its current performance. This assessment helps us identify the keywords for which your website is currently ranking, which are valuable assets for your AdWords campaign. Our goal is to enhance your effectiveness for these keywords and maximize their potential.`
                },
                para5: {
                    description: `Additionally, we identify keywords where your performance is lacking and devise strategies to improve them. Effective keyword strategy development relies on understanding market dynamics, making keyword research a critical step in the process.`
                },
                para6: {
                    description: `After conducting internal and external keyword research, Savvy Ray Technologies compiles your keyword list. We input this list into Google Keyword Planner, where we analyze various factors such as search volume, competition, cost per click, region, language, and other relevant data. This in-depth analysis guides us in creating your final keyword strategy, which will be implemented in your AdWords campaign. You can consider this phase the culmination of your keyword research, paving the way for successful campaign execution.`
                },
                para7: {
                    description: `With over 2 years of experience, our AdWords team at Savvy Ray Technologies has expertise in various sectors. We utilize proven methodologies to determine when to use AdWords and when to employ organic (SEO) strategies for optimal results. As a leading SEO company in Ahmedabad and the United States, we stay updated on global trends. If you have any questions regarding keyword research and analysis, feel free to contact us.`
                },
                para8: {
                    description: `Our Google Ads Services include:`,
                    list: [
                        '● Keyword research and selection',
                        '● Competitive research',
                        '● Optimization of landing pages with engaging text and image ads',
                        '● PPC cost control',
                        '● PPC tracking',
                        '● Continuous improvement and enhancements to ad campaigns',
                        '● Conversion tracking',
                        '● Monthly reports',
                    ]
                },
                para9: {
                    description: `Please reach out to us for top-notch Google Ads services.`
                },
                para10: {
                    title: ` Why Choose Savvy Ray Technologies for Google Ads Services?`,
                    description: `If you've been using Google Ads to promote your online business and haven't achieved the desired results despite significant spending, it's time to hire a skilled Google Ads specialist. At Savvy Ray Technologies, we can help you eliminate wasted budget, maximize your return on investment, and drive quality and potential visitors to your website.`
                },
                para11: {
                    description: `Instead of focusing on increasing spending, our approach is to generate meaningful traffic that delivers tangible results. With our expertise and services, we ensure that your products reach potential customers among the billions of searches conducted on Google every day. Effective ad management requires extensive knowledge and skill, which not every company possesses.`
                },
                para12: {
                    description: `We have successfully collaborated with numerous companies, ranging from startups to large corporations, and have consistently delivered proven results with a 100% success rate. There's no need to waste your money or efforts when Savvy Ray can handle it for you!`
                },
                para13: {
                    description: `Choose Savvy Ray Technologies today and experience the difference in your Google Ads campaigns.`
                }
            }
        }
    }
}
</script>