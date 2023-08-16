<template>
    <div class="row row--15 service-wrapper">
        <div class="col-lg-4 col-md-6 col-sm-6 col-12"
             v-for="(service, index) in serviceList"
             :key=index>
            <div class="service service__style--1 bg-color-blackest radius mt--25 text-start"
                 data-aos="fade-up"
                 data-aos-delay="70">
                <div class="icon" v-if="service.icon">
                    <Icon :name="service.icon" class="size-62"/>
                </div>
                <div class="content">
                    <h4 class="title w-600">
                        {{ service.title }}
                    </h4>
                    <p class="description b1 color-gray mb--0" v-html="service.description"/>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import Icon from '@/components/icon/Icon'

    export default {
        name: 'Cards',
        components: {Icon},
        props: {
            serviceList: {
                type: Array,
                default: []
            }
        }
    }
</script>