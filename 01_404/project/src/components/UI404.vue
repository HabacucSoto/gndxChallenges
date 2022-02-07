<template>
    <div class="cont container d-flex justify-content-around 
    align-items-center flex-column flex-md-row">
        <div>
            <img src="../assets/404.png" alt="ERROR 404" title="ERROR 404">
        </div>
        <div class="d-flex flex-column align-items-center">
            <h1>¡I have bad news for you!</h1>
            <h3>Sorry, the page you requested does not exist :(</h3>
            <router-link to="/" class="btn btn-dark w-50">H O M E</router-link>
        </div>
    </div>
</template>

<script>
export default {
    name: 'UI404'
}
</script>

<style scoped>
    *{
        font-family: monospace;
        font-weight: 600;
    }
    .cont {
        height: 80vh;
    }
    img {
        animation: astro 5s linear infinite;
        z-index: -45445;
    }
    @keyframes astro{
        0%{
            margin-top: -10px;
        }
        25%{
            margin-top: 0;
        }
        50%{
            margin-top: 10px;
        }
        75%{
            margin-top: 0;
        }
        100%{
            margin-top: -10px;
        }
    }
</style>