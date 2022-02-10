<template>
<div class="header-Section"> 
    <div class="header-info d-flex justify-content-between">
            <div>
                <i class="fas-fa fa-clock"></i>
                <span>Open Hours Mon - Sat - 0.00 - 18.00</span>
            </div>
            <div class="header-contact d-flex">
            <span class="px-2" >+1 (305) 1234 5678</span>
            <span class="px-2">hello@axample.com</span>
            </div>    
        </div>
    <header>
          
        <nav class="d-flex justify-content-between py-3">
        <div class="title">
            <span class="nex">NEX</span>
            <span class="gen">GEN</span>
        </div>
            <ul>
                <li class="px-4 py-2" v-for="nav in header" :key="nav.id">{{nav.label}}</li>
                <li class=" get-in-touch px-4 py-2">GET IN TOUCH</li>
            </ul>
        </nav>
        <div class="header-content d-flex flex-column justify-content-center">
            <div class="h-res">HUMAN RESOURCES</div>
            <span class="">
                <p class="get-more">Get More</p>
                <span class="productivity">Productivity</span>
                 
            </span>
            <div class="subtitle">Planning, recruiment and selection process and performance evaluation of employees</div>
            <div class="header-button d-flex my-4">
                <div class="get-in-touch px-4 py-2">GET IN TOUCH</div>
                <div class="read-more px-4 py-2 mx-3"> READ MORE</div>
            </div>
        </div>
    </header>
</div>
</template>

<script>
export default {
    data() {
        return {
            header:[
                {
                    id: '1',
                    label: 'HOME',
                },

                {
                    id: '2',
                    label: 'ABOUT',
                },

                {
                    id: '3',
                    label: 'PROJECTS',
                },

                {
                    id: '4',
                    label: 'TESTIMONIALS',
                },

                {
                    id: '5',
                    label: 'OMINO',
                },

                

            ]
        }
    }
    
}
</script>

<style scoped lang="scss">
@import "@/style/general.scss"; //scss generale -- Bootsrap -- Fontawesome
@import "@/style/header.scss";
</style>
