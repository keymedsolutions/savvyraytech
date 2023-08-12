<template>
    <Layout :show-cta="false">
        <!-- Start Contact Area  -->
        <div class="rwt-contact-area rn-section-gap">
            <div class="container">
                <div class="row">
                    <div class="col-lg-12 mb--40">
                        <SectionTitle
                            text-align="center"
                            subtitle="Contact Form"
                            title="Contact Us"
                        />
                    </div>
                </div>

                <div class="row mt--40 row--15 justify-content-center">
                    <div class="col-lg-8">
                        <ContactForm/>
                    </div>
                </div>
            </div>
        </div>
        <!-- End Contact Area  -->
    </Layout>
</template>

<script>
    import Layout from '@/components/common/Layout'
    import Breadcrumb from '@/components/elements/breadcrumb/Breadcrumb'
    import SectionTitle from '@/components/elements/sectionTitle/SectionTitle'
    import Icon from "@/components/icon/Icon";
    import GoogleMap from "@/components/elements/contact/GoogleMap";
    import ContactForm from "@/components/elements/contact/ContactForm";

    export default {
        name: 'ContactPage',
        components: {ContactForm, GoogleMap, Icon, SectionTitle, Breadcrumb, Layout}
    }
</script>