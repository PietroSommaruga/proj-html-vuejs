<template>
<div class="main-first">
    <div class="three-box-container d-flex justify-content-between align-items-center">
        <div class="card" v-for="card in threeCard" :key="card.id">
            <h3>{{card.title}}</h3>
            <p>{{card.text}}</p>
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
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import "@/style/main-first.scss";

</style>
