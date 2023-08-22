<template>
    <div class="container">
        <div class="row row--15 service-wrapper">
            <div class="col-lg-3 col-md-6 col-sm-6 col-12"
                v-for="(service, index) in serviceList"
                :key=index>
                <div class="service service__style--1 icon-circle-style with-working-process text-center"
                    data-aos="fade-up"
                    data-aos-delay="70">
                    <div class="icon">
                        <div class="line"/>
                        {{ service.icon }}
                    </div>
                    <div class="content">
                        <h4 class="title">
                            {{ service.title }}
                        </h4>
                        <p class="description b1 color-gray mb--0" v-html="service.description"/>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Flow',
        props: {
            serviceList: {
                type: Array
            }
        }
    }
</script>