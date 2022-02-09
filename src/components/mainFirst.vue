<template>
<div class="main-first">
    <div class="three-box-container d-flex justify-content-between align-items-center">
        <div class="card px-4 d-flex flex-column justify-content-center" v-for="card in threeCard" :key="card.id">
            <h3>{{card.title}}</h3>
            <p>{{card.text}}
            </p>
        </div>
    </div>

    <div class="the-company d-flex">
        <div class="text d-flex flex-column justify-content-center ">
            <strong class="about">ABOUT THE NETWORK</strong>
            <strong class="title-section my-3">
                <span class="the px-2">The</span>
                <span class="px-2">Company</span>
            </strong>
            <p class="subtitle">Lorem ipsum dolor sit amet consectetur numquam  recusandae quasi ex dolor eos. Perspiciatis dolores asperiores dolor cum.</p>
            <div class="block-container d-flex justify-content-between pt-3 ">
                <div class="block d-flex flex-column pb-3" v-for="block in threeCardB" :key="block.id">
                    <strong class="block-counter px-3 py-1">{{block.counter}}</strong>
                    <h4>{{block.category}}</h4>
                    <span class="block-text">{{block.text}}</span>
                </div>
            </div>
            <div class="button-container d-flex pt-5">
                <button class="get-in-touch py-3 px-5 mx-2">GET IN TOUCH</button>
                <button class="read-more py-3 px-5 mx-2">READ MORE</button>
            </div>
        </div>
        <div class="img">
            <img src="@/assets/about-5.jpg" alt="">
        </div>
    </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            threeCard:[
                {
                    id: '1',
                    icon: '',
                    title: 'Human Capital',
                    text: 'Humanizing business: Harness the power of technology to improve the way peaople work.',
                },

                {
                    id: '2',
                    icon: '',
                    title: 'Core Business',
                    text: 'It takes innovative approaches to transform, modernize, and run existing platforms.',
                },

                {
                    id: '3',
                    icon: '',
                    title: 'Performance',
                    text: 'Archieving maximum impact and value from investments in finance and supply chain.',
                },
            ],
            threeCardB:[
                {
                    id: '1',
                    counter: '0',
                    category: 'Employees',
                    text: 'lorem ipsum dolor sit amet',
                },

                {
                    id: '2',
                    counter: '0',
                    category: 'Partners',
                    text: 'Lorem, ipsum dolor sit',
                },

                {
                    id: '3',
                    counter: '0',
                    category: 'Customers',
                    text: 'Lorem, ipsum dolor sit',
                },
            ],
            
        }
    }
}
</script>

<style scoped lang="scss">
@import "@/style/main-first.scss";

</style>
