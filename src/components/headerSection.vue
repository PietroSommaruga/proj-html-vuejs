<template>
<div class="header-Section"> 
    <div class="header-info d-flex justify-content-between">
            <span>Open Hours Mon - Sat - 0.00 - 18.00</span>
            <div class="header-contact d-flex">
            <span class="px-2" >+1 (305) 1234 5678</span>
            <span class="px-2">hello@axample.com</span>
            </div>    
        </div>
    <header>
          
        <nav class="d-flex justify-content-between py-3">
        <span>NEXGEN</span>
            <ul>
                <li class="px-2" v-for="nav in header" :key="nav.id">{{nav.label}}</li>
                <li class=" get-in-touch">GET IN TOUCH</li>
            </ul>
        </nav>
        <div class="header-content d-flex flex-column justify-content-center">
            <div>HUMAN RESOURCES</div>
            <h1>Get More Productivity</h1>
            <p>Planning, recruiment and selection process and performance evaluation of employees</p>
            <div class="header-button">
                <button>GET IN TOUCH</button>
                <button> READ MORE</button>
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
@import "@/style/header.scss";
</style>
