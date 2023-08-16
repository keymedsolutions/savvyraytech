<template>
    <Layout header-class="header-transparent" buy-button-class="btn-default btn-small">
        <Breadcrumb :current-url="name" :title="name"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="seoData.para1" :noDescriptionMargin="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="seoData.para2" :showList="true"/>
        <TextComponent data-aos="fade-up" data-aos-delay="100" :data="seoData.para3" :noDescriptionMargin="true"/>
        <Separator />
        <div class="container mb--60 mt--60">
            <div class="row">
                <div class="col-md-6">
                    <Accordian :title="accordianData1.title" :data="accordianData1.data" />
                </div>
                <div class="col-md-6">
                    <Accordian :title="accordianData2.title" :data="accordianData2.data" />
                </div>
            </div>
        </div>
        <Separator />
        <section class="rn-service-area rn-section-gap">
            <div class="container">
                <div class="row row--30">
                    <div class="col-lg-12">
                        <SectionTitle
                            class="mb--30"
                            text-align="center"
                            subtitle="Maximize Your Online Visibility with Improved Search Rankings"
                            title="Our SEO Services"
                            data-aos="fade-up"
                            data-aos-delay="60"
                        />
                    </div>
                </div>
                <Cards :serviceList="serviceList"/>
            </div>
        </section>
        <Separator />
        <div class="container pt--60 pb--60">
            <div class="row">
                <Accordian :title="faq.title" :data="faq.data" />
            </div>
        </div>
    </Layout>
</template>
<script>
import Breadcrumb from '@/components/elements/breadcrumb/Breadcrumb.vue';
import Layout from "../../components/common/Layout";
import TextComponent from '@/components/custom/textComponent.vue';
import Separator from '@/components/elements/separator/Separator'
import Accordian from '@/components/custom/accordian.vue';
import SectionTitle from '@/components/elements/sectionTitle/SectionTitle';
import Cards from '@/components/custom/cards.vue';

export default {
    name: 'SearchEngineOptimization',
    components: {Layout, Breadcrumb, TextComponent, Separator, Accordian, SectionTitle, Cards},
    data() {
        return {
            name: 'Search engine optimization',
            seoData: {
                para1: {
                    title: 'An SEO Marketing Company That Understands Your Needs',
                    description: 'At Savvy Ray Technologies, we understand that you have a clear vision of your needs, but you may be unsure of how to achieve them. Our SEO specialists have heard this from numerous clients like you.'
                },
                para2: {
                    list: [
                        '● Your website is struggling to gain online visibility.',
                        "● Your website traffic has recently declined, and you're unsure why.",
                        "● The volume of incoming calls and leads has suddenly decreased.",
                        "● You're launching a new website and seeking quick business growth."
                    ],
                    description: "If any of these four pain points resonate with you, be assured that you've found the right SEO company."
                },
                para3: {
                    description: "Savvy Ray Technologies is currently serving numerous SEO clients and delivering optimization solutions to address Google's constantly evolving algorithm."
                }
            },
            accordianData1: {
                title: 'How SEO Can Transform Your Business?',
                data: [
                    {
                        id: 'One',
                        title: 'Increase Revenue with Organic Traffic',
                        description: 'Experience a substantial boost in revenue through increased organic traffic to your website.'
                    },
                    {
                        id: 'Two',
                        title: 'Enhance Online Brand Presence',
                        description: "Elevate your brand's image and online recognition with optimal search engine rankings, creating a positive brand presence."
                    },
                    {
                        id: 'Three',
                        title: 'Drive Sales Growth',
                        description: 'Increase the chances of converting leads into sales by attracting more prospects to your website and maximizing sales opportunities.'
                    },
                    {
                        id: 'Four',
                        title: 'Accelerate Business Growth',
                        description: 'With our SEO services in the US and Ahmedabad, businesses can expect rapid growth and make a significant industry impact.'
                    }
                ]
            },
            accordianData2: {
                title: ' Your Journey with Savvy Ray Technologies',
                data: [
                    {
                        id: 'a2-1',
                        title: 'Analysis ',
                        description: 'At the start of your SEO journey with us, we analyze your website to identify areas that require attention and gain a comprehensive understanding of your overall traffic and individual page performance.'
                    },
                    {
                        id: 'a2-2',
                        title: 'Research',
                        description: "Next, we conduct thorough research, exploring your competition, studying the market landscape, performing keyword research, and gaining valuable insights into your potential customers' expectations."
                    },
                    {
                        id: 'a2-3',
                        title: 'Optimization',
                        description: "With the knowledge gained, we move into the optimization phase, developing tailored SEO strategies that cater to your specific needs. This includes both on-page and off-page optimization techniques, as well as strategic content marketing."
                    },
                    {
                        id: 'a2-4',
                        title: 'Reporting',
                        description: "Throughout the process, we prioritize transparency and collaboration. Our team provides regular reporting, delivering monthly updates on the progress of your SEO campaign. This empowers you to track the results and stay actively involved in the journey toward improving your online presence."
                    }

                ]
            },
            serviceList: [
                {
                    title: 'Local Business Listing',
                    description: 'Expand your reach and engage your local audience with our expertise in managing online business listings on platforms like Google+ Local, ensuring maximum visibility and connection with your city.'
                },
                {
                    title: 'Google Analytics',
                    description: 'Gain valuable insights into user preferences and behavior with the power of Google Analytics. Our team will help you leverage this tool to enhance your SEO strategies and achieve better results.'
                },
                {
                    title: 'Google Search Console',
                    description: 'Uncover valuable data and identify areas for improvement with the Google Search Console. Our SEO experts will guide you in utilizing its tools effectively, driving success and enhancing your online presence.'
                },
                {
                    title: 'Link Building',
                    description: "Boost your website's popularity and online presence through strategic link building partnerships. Even if you're starting from scratch, we help you establish valuable connections with high-traffic websites."
                },
                {
                    title: 'Page Speed Optimization',
                    description: "Don't let slow-loading websites hinder your search engine rankings. Our optimization techniques ensure your website loads quickly, pleasing both visitors and search engines for better performance."
                },
                {
                    title: 'Schema Implementation',
                    description: 'Optimize your website content for quality search engine result pages (SERPs) with Schema Markup. We enhance the understanding and categorization of your content, improving visibility and relevance.'
                },
                {
                    title: 'On-Site SEO',
                    description: 'Drive organic traffic to your website and boost lead generation with our specialized on-site SEO services. We optimize your website by incorporating high-ranking keywords and relevant elements that attract and convert visitors.'
                },
                {
                    title: 'Conversion Optimization',
                    description: "Maximize your conversion rates through our result-oriented techniques, including split testing, workflow improvement, and content enhancement. Generate more leads and increase website traffic effectively."
                },
                {
                    title: 'SEO Consulting Services',
                    description: "As an SEO service provider in Ahmedabad, we offer cost-effective and ROI-based consulting services. With our expertise, we help your brand make a wide-reaching impact and generate profitable results in the ever-growing digital world."
                },
                {
                    title: 'Blog Creation',
                    description: "Enhance your content marketing efforts with a captivating and informative blog. Our team will create a tailored blog for your niche, attracting organic traffic and increasing your online visibility."
                },
                {
                    title: 'Social Media Circulation',
                    description: "Harness the power of social media and create a viral presence that drives potential customers to your website. Achieve high revenue generation through engaging and shareable content."
                },
                {
                    title: 'Content Optimization',
                    description: "Ensure your great content generates revenue by optimizing it strategically. Our experts optimize your content to maximize its visibility, relevance, and impact on your target audience."
                },
                {
                    title: 'Mobile Optimization',
                    description: "Cater to the mobile-centric world by optimizing your website for flawless performance on smartphones and tablets. Don't miss out on potential customers browsing on mobile devices."
                },
                {
                    title: 'Website Structure Optimization',
                    description: "Achieve higher search engine rankings and click-through rates with our advanced website optimization strategies. We optimize your website's structure to increase its overall performance and user engagement."
                },
            ],
            faq: {
                title: 'Frequently Asked Questions',
                data: [
                    {
                        id: 'FAQ-1',
                        title: 'What is SEO?',
                        description: `SEO, or search engine optimization, is an essential practice that aims to optimize websites for better visibility in Google search results, leading to increased web traffic and improved rankings in SERPs. It involves a multifaceted approach that encompasses various strategies, such as meticulous keyword selection, crafting high-quality content, and establishing strong backlinks. While SEO may seem intricate and time-consuming, the rewards it offers are well worth the investment. By investing in effective SEO techniques, you can attract a more targeted audience to your website and unlock its full potential.<br/><br/> Discover the power of SEO for your business and unlock new horizons. Contact us today to explore our exceptional SEO services tailored to your unique needs.`
                    },
                    {
                        id: 'FAQ-2',
                        title: 'How long does SEO take before I see the benefits?',
                        description: `"Those who wait for good things will find them."<br/><br/>Perhaps you've come across an SEO company that guarantees quick results. Sorry to break the news to you, but they are all scams. Results from organic SEO services carried out ethically won't come quickly. It should typically take three to six months before you notice significant development on your website.`
                    },
                    {
                        id: 'FAQ-3',
                        title: 'How do i know if my SEO campaign is making progress?',
                        description: `You will receive monthly reports from us. In this manner, you may monitor the development of your SEO effort.`
                    },
                    {
                        id: 'FAQ-4',
                        title: 'What is an average budget for SEO?',
                        description: `In India, the price of SEO ranges from Rs. 25,000 to Rs. 1,20,000 a month. Despite the fact that the task is the same, the pace varies greatly according to 1) The expertise of the person who prepares the SEO plan. 2) The time it takes ONE person to complete ONE task. Fewer employees are deployed on your account to complete the task if your budget is lower.`
                    }
                ]
            }
        }
    }
}
</script>