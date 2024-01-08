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
            <p class="brand-name d-flex mr-n16 ml-n6"><p class="mr-2" style="color: #8b2627;">Salutar</p> Clínica</p>
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

.brand-name{
  font-family: 'Times New Roman', Times, serif !important;
  font-size: 40px;
}

</style>