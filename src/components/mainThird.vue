<template>
<div>
    <div class="management-container d-flex flex-column align-items-center justify-content-center">
        <strong class="how">HOW IT WORKS IN PRATICE</strong>
        <div class="title-section">
            <strong class="process px-3 mx-1">Process</strong>
            <strong class="mx-1">Management </strong>
        </div>
        <p class="subtitle my-4">We work with innovative methodologies to ensure that the entre reformatting process is done from start to finish as planned</p>
        <div class="pallini d-flex justify-content-around mt-5">
            <div class="pallino">01</div>
            <div class="pallino">01</div>
            <div class="pallino">01</div>
            <div class="pallino">01</div>
            <div class="pallino">01</div>
        </div>
        <div class="sotto-pallino d-flex justify-content-around">

            <div class="pallino-title">
                <h3 class="py-4">Collection of information</h3>
                <p>Lorem ipsum dolor sit amet consectetur.</p>
            </div>
            <div class="pallino-title">
                <h3 class="py-4">Strategic planning</h3>
                <p>Lorem ipsum dolor sit amet consectetur.</p>
            </div>
            <div class="pallino-title">
                <h3 class="py-4">Assignment of responsabilities</h3>
                <p>Lorem ipsum dolor sit amet consectetur.</p>
            </div>
            <div class="pallino-title">
                <h3 class="py-4">Formatting process</h3>
                <p>Lorem ipsum dolor sit amet consectetur.</p>
            </div>
            <div class="pallino-title">
                <h3 class="py-4">Continuity formalization</h3>
                <p>Lorem ipsum dolor sit amet consectetur.</p>
            </div>

        </div>

    </div>

<!-- ------------------------------------------------- -->

    <div class="trusted-feedback-container d-flex flex-column align-items-center justify-content-center">
        <strong class="testimonials py-2">CUSTOMER TESTIMONIALS</strong>
        <div class="title-section">
            <strong>Trusted</strong>
            <strong class="feedback px-3 mx-3">Feedback</strong>
        </div>
        <p class="feed py-3">We work intensively of ideas that can add up in the lives of our costumers. This is what moves us and we are grateful for the recognition.</p>
        <div class="feedback-container d-flex justify-content-between">
            <div class="feedback p-5" v-for="feedback in feedbacks" :key="feedback.id">
                <img :src="require('@/assets/' + feedback.img)" alt="">
                <p class="py-3">{{feedback.feed}}</p>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            feedbacks:[
                {
                    id: '1',
                    name:'woocommerce',
                    img: 'logo-1.png',
                    feed:'Consectetur adipisicing elit. consectetur adipisicing elit voluptates odit optio illum impedit, vero nihil ad deserunt? Lorem Soluta consequuntur sit voluptates odit optio vero ab fuga earum in amet minima quasi illum impedit, eligendi sequi omnis nihil ad deserunt?'
                },

                {
                    id: '2',
                    name:'wordpress',
                    img: 'logo-2.png',
                    feed:"Amet . Soluta consequuntur sit  ab fuga earum in amet minima quasi  eligendi sequi omnis  ipsum dolor sit, amet consectetur adipisicing elit. Consequatur autem eum iusto quo, corporis, possimus, quidem praesentium expedita odio eius impedit id modi quaerat numquam voluptates aspernatur?"
                },

                {
                    id: '3',
                    name:'woocommerce',
                    img: 'logo-3.png',
                    feed:'Odit optio vero ab fuga earum in amet minima quasi illum impedit, eligendi sequi omnis nihil ad deserunt? sit, amet consectetur adipisicing elit. Consequatur autem eum iusto quo, corporis, possimus, quidem praesentium expedita odio eius impedit id modi quaerat voluptatem numquam aspernatur?'
                },


            ],
        }
    }
}
</script>

<style scoped lang="scss">
@import "@/style/main-third.scss";
</style>


