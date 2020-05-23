<template>
  <v-container fluid>
    <v-card>
      <v-card-text>
        <h3>Bienvenido Usuario</h3>
      </v-card-text>
      <v-card-text>
        <div class="text-right">
          <v-chip>
            <v-avatar>
              <img src="https://cdn2.salud180.com/sites/default/files/styles/medium/public/field/image/2016/07/beard1_0.jpg" alt="trevor">
            </v-avatar>Mensaje de Chat
          </v-chip>
          <p class="caption mr-2">06 febrero 2019 10am</p>
        </div>
      </v-card-text>
      <v-card-text>
        <v-form @submit.prevent="enviarMensaje"> 
          <v-text-field v-model="mensaje" label="Escribe tu mensaje aqui"></v-text-field>
        </v-form>
      </v-card-text>
    </v-card>
  </v-container>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
  },
  data(){
    return{
      mensaje:''
    }
  },
  methods:{
    enviarMensaje(){
      console.log('Enviaste el mensaje: ', this.mensaje)
    }
  }
}
</script>
