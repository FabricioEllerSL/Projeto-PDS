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
            <v-col cols="8">
                <h3 class="text-center text-secondary text-h3 font-weight-bold mt-10">Bem Vindo, XXXXXX!</h3>
                <p class="mx-auto text-center mt-8 text-h6 text-grey clique-modulos-texto">Clique em um dos módulos para acessar suas funções.</p>
            </v-col>
            <v-col cols="2">

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

.clique-modulos-texto{
    width: 300px;
}

</style>