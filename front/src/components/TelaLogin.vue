<script>
    export default{
        name: 'TelaLogin',
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
    <div>
        <nav class="nav-bar d-flex justify-space-between align-center px-16">
            <p class="brand-name d-flex mr-n16 ml-n6"><p class="mr-2" style="color: #8b2627;">Salutar</p> Clínica</p>
            <v-text>PsychoSystem &copy; 2023</v-text>
            <v-text>{{ dataAtual }}</v-text>
        </nav>

        <v-row>
            <v-col class="d-flex align-center justify-center">
                <v-card elevation="10" class="bg-white w-75 h-75 login-card d-flex align-center justify-center">
                    <div class="text-center w-75">
                        <h1 class="text-brown text-h2 font-weight-bold">Login</h1>
                        <h2 class="text-grey text-subtitle-1">Entre para continuar</h2>
                        <v-form class="mt-10">
                            <v-text-field :rules="rules" label="Nome"></v-text-field>
                            <v-text-field :rules="rules" label="Senha"></v-text-field>
                            <v-btn type="submit" class="mt-2 w-75 bg-third text-white">Submit</v-btn>
                        </v-form>
                    </div>
                </v-card>
            </v-col>
            <v-col>
              <v-img class="w-75 mt-10" src="@/assets/candlestick.png" alt="" />
            </v-col>
        </v-row>
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

.login-card{
    border-radius: 50px !important;
}

</style>