<script>
    export default{
        name: 'ModulosGerente',
        data(){
            return{
                dataAtual: new Date().toLocaleDateString(),
                rules: [
                    value => {
                    if (value) return true

                    return 'Campo Necessário'
                    },
                ],
            }
        }
    }
</script>

<template>
    <v-container fluid class="ma-0 pa-0">
        <nav class="nav-bar d-flex justify-space-between align-center px-16">
            <p class="brand-name d-flex mr-n16 ml-n6"><p class="mr-2" style="color: #8b2627;">Salutar</p> Clínica</p>
            <p>PsychoSystem &copy; 2023</p>
            <p class="text-h6">GERENTE</p>
        </nav>

        <v-row>
            <v-col cols="2">
                <p><img src="@/assets/icons/chevron-left.png" alt=""></p>
            </v-col>
            <v-col cols="10">
                <h3 class="w-25 mx-auto">Bem Vindo, XXXXXX!</h3>
            </v-col>
        </v-row>
    </v-container>
</template>

<style scoped>
.nav-bar{
    background-color:  #fff;
    margin: 0;
    height: 70px;
    opacity: 1;
}

.brand-name{
  font-family: 'Times New Roman', Times, serif !important;
  font-size: 40px;
}

</style>