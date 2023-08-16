<template>
     <Layout header-class="header-transparent" buy-button-class="btn-default btn-small">
        <Breadcrumb :current-url="name" :title="name"/>
    </Layout>
</template>
<script>
import Breadcrumb from '@/components/elements/breadcrumb/Breadcrumb.vue';
import Layout from "../../components/common/Layout";

export default {
    name: 'Branding',
        components: {Layout, Breadcrumb},

    data() {
        return {
            name: 'Branding'
        }
    }
}
</script>