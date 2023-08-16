<template>
     <Layout header-class="header-transparent" buy-button-class="btn-default btn-small">
        <Breadcrumb :current-url="name" :title="name"/>
    </Layout>
</template>
<script>
import Breadcrumb from '@/components/elements/breadcrumb/Breadcrumb.vue';
import Layout from "../../components/common/Layout";

export default {
    name: 'ConceptShoots',
        components: {Layout, Breadcrumb},

    data() {
        return {
            name: 'Concept shoots'
        }
    }
}
</script>