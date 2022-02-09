<template>
<div class="actions-container">
    <p>WE DO MORE FOR EVERYONE</p>
    <h1>Actions & Projects</h1>
    <nav>
        <ul class="d-flex justify-content-center py-3">
            <li class="px-3 py-2" v-for="project in projects" :key="project.id">{{project.type}}</li>
        </ul>
    </nav>
    <div class="card-container d-flex flex-wrap justify-content-between" >
        <div class="card my-4" v-for="project in projects" :key="project.id">
            <img :src="require('@/assets/' + project.img)" alt="">
            <strong class="text px-4">{{project.text}}</strong>
        </div>
    </div>    
    <!-- <div>{{project[currentIndex].type}}</div> -->
</div>

</template>

<script>
export default {
    
    data() {
        return {
            projects:[
                // {
                //     id: '1',
                //     type: 'ALL',
                // },

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
            // selectedValue: '',
        }
    },
    methods: {
    // ----- filtro per genere -----
    // filterGenre(selectedValue) {
    //   if (selectedValue === 'All') {
    //     this.projects = this.project;
    //   } else {
    //     this.projects = this.project.filter((project) => {
    //       return project.type.includes(selectedValue); 
    //     });
    //   }
    // },
  }
}
</script>

<style scoped lang="scss">
@import "@/style/main-second.scss";
</style>
