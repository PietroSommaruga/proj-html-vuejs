<template>
<footer class="d-flex">
    <div class="footer-left d-flex flex-column justify-content-center">
        <span class="send">SEND A MESSAGE</span>
        <div class="title-section">
            <strong class="">Get in</strong>
            <strong class="touch mx-3 px-3">Touch </strong>
        </div>
        <p class="respond my-4">We will respond to your message as soon as possible.</p>
        <div class="input-1 my-1">
            <input class="px-2" type="text" placeholder="Name">
            <input class="ml px-2" type="text" placeholder="Email">
        </div>
        <div class="input-2 my-1">
            <input class="px-2" type="text" placeholder="Phone">
            <select class="ml px-2" name="" id="" placeholder="More info">
                <option value="More info">More info</option>
                <option value="Our email">Our email</option>
                <option value="Other contact">Other contact</option>
                <option value="All sources">All sources</option>
                <option value=""></option>
            </select>
        </div>
        <div class="input-3 my-1" my-1>
            <textarea class="px-2" name="" id="" rows="10" placeholder="Message"></textarea>
        </div>
        <div>
            <button class="send-button px-4 py-2">SEND</button>
        </div>
    </div>
    <div class="footer-right d-flex flex-column justify-content-center">
        <h3>Example Inc</h3>
        <p>Lorem ipsum dolor sit, amet consectetur  iusto! Sint tempore, totam aspernatur dolorum architecto omnis!</p>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Culpa optio adipisci id? Corrupti iusto! Sint tempore, totam.</p>

        <div class="contancts d-flex flex-column justify-content-center"> 
            <span>+1 (305) 1234-5678</span>
            <span>hello@example.com</span>
            <span>Main Avenue, 987 Miami</span>
        </div>
        <div>
            <button class="view-button px-4 py-2 my-2">VIEW MAP</button>
        </div>



    </div>
</footer>
</template>

<script>
export default {
    
}

</script>

<style scoped lang="scss">
@import "@/style/footer.scss";

</style>
