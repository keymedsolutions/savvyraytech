<template>
    <div class="rn-splite-style">
        <div class="split-wrapper">
            <div class="row no-gutters radius-10 align-items-center justify-content-center">
                <div class="col-lg-8 col-xl-8 col-8">
                    <div class="split-inner">
                        <h4 class="title" v-if="data.title">{{ data.title }}</h4>
                        <p class="description">{{ data.description }}</p>
                        <ul class="split-list" v-if="showList">
                            <li v-for="(listItem, index) in data.list" :key='index'>{{ listItem }}</li>
                        </ul>
                        <div class="view-more-button mt--35" v-if="data.btn">
                            <Button :title="data.btn.text" :url="data.btn.link"/>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import Button from '@/components/elements/button/Button'
    import Counter from '@/components/elements/counterUp/Counter'

    export default {
        name: 'TextComponent',
        components: {Counter, Button},
        props: {
            showList: {
                type: Boolean,
                default: false
            },
            data: {}
        }
    }
</script>