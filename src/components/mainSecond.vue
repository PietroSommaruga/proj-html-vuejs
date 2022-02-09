<template>
<div class="actions-container">
    <p>WE DO MORE FOR EVERYONE</p>
    <div class="title-section">
        <strong>Actions &</strong>
        <strong class="projects px-3 mx-3">Projects </strong>
    </div>
    <nav>
        <ul class="d-flex justify-content-center py-3">
            <li class="px-3 py-2">ALL</li>
            <li class="px-3 py-2" v-for="project in projects" :key="project.id">{{project.type}}</li>
        </ul>
    </nav>
    <div class="card-container d-flex flex-wrap justify-content-between" >
        <div class="card my-4" v-for="project in projects" :key="project.id">
            <img :src="require('@/assets/' + project.img)" alt="">
            <strong class="text px-4">{{project.text}}</strong>
        </div>
    </div>    
</div>

</template>

<script>
export default {
    
    data() {
        return {
            projects:[
                {
                    id: '2',
                    type: 'INSTITUTIONAL',
                    img: 'about-5.jpg',
                    text:'Academic professional program in social media'
                },

                {
                    id: '3',
                    type: 'SOCIAL',
                    img: 'project-2.jpg',
                    text:"President's speech at the annual meeting"
                },

                {
                    id: '4',
                    type: 'EVENTS',
                    img: 'project-3.jpg',
                    text:'International business trip in Shangai'
                },

                {
                    id: '5',
                    type: 'INNOVATION',
                    img: 'project-4.jpg',
                    text:'Technology workshop whit education theme'
                },

                {
                    id: '6',
                    type: 'ENVIROMENT',
                    img: 'project-5.jpg',
                    text:'Donation of clothes and food to the partner NGO'
                },

                {
                    id: '7',
                    type: 'TECHNOLOGY',
                    img: 'project-6.jpg',
                    text:'Confraternization of the procurement team'
                },

            ],
        }
    },
    methods: {
  }
}
</script>

<style scoped lang="scss">
@import "@/style/main-second.scss";
</style>
