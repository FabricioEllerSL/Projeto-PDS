<script>
    export default{
        name: 'TelaLogin',
        data(){
            return{
                dataAtual: new Date().toLocaleDateString(),
            }
        }
    }
</script>

<template>
    <div>
        <nav class="nav-bar d-flex justify-space-between align-center px-16">
            <v-btn to="/" class="rounded-xl px-8 login-button">Início</v-btn>
            <v-text>PsychoSystem &copy; 2023</v-text>
            <v-text>{{ dataAtual }}</v-text>
        </nav>
    </div>
</template>

<style scoped>
.nav-bar{
    background-color:  #fff;
    margin: 0;
    height: 70px;
    opacity: 1;
}

.login-button{
    background-color: #edd7dd !important;
    color: #555;
    font-size: 20px;
}    
</style>