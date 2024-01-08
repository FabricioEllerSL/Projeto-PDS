<script>
    export default{
        name: 'TelaPrincipal',
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
            <v-btn to="/login" class="rounded-xl px-8 login-button">LOGIN</v-btn>
            <v-text>PsychoSystem &copy; 2023</v-text>
            <v-text>{{ dataAtual }}</v-text>
        </nav>
        <v-main>
          <v-row>
            <v-col class="pa-0">
              <p class="ml-16 mt-16 pl-16 mb-n9 pt-16 text-h1 font-times" style="color: #913132;">Salutar</p>
              <p class="ml-16 mt-16 pl-16 text-h1 font-times" style="color: #5b442f;">Clínica <img class="leaves-image ml-n10 mt-n16 mb-n16" src="@/assets/leaves.png" alt="Folhas Logo"></p>
              <p class="text-h5 ml-16 pl-16 mt-16 font-weight-light">Sistema de gerenciamento de informações.</p>
            </v-col>
            <v-col>
              <v-img class="w-75 mt-10" src="@/assets/candlestick.png" alt="" />
            </v-col>
          </v-row>
        </v-main>
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


.leaves-image{
  height: 200px;
}

.font-times{
  font-family: 'Times New Roman', Times, serif !important;
}

</style>