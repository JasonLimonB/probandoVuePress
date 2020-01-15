<template>
    <div>
        <ul>
            <li v-for="message in messages">
                <h3>{{ message.title }}</h3>
                <p>{{ message.text }}</p>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'Helloworld',
    data(){
        return{
            messages: [
                {
                    title:'Curso Vuejs',
                    text: 'Un excelente Framework que estoy descubriendo y me está encatado'
                },
                {
                    title: 'Curso Angular',
                    text: 'Framework creado por google que es uno de mis favoritos'
                }
            ]
        }
    }
}
</script>

<style scoped>
    li{
        display: block;
        max-width: 300px;
        margin: 0 auto;
        box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.3);
        padding: 1em;
        border-radius: 8px;
    }
</style>