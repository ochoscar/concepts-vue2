<template>
  <v-app>
    <v-app-bar color="primary" dark app>
        <span>{{ titulo }}</span>
    </v-app-bar>
    
    <v-main>
      <v-container fluid fill-height>
        <create-user></create-user>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
  import CreateUser from './components/CreateUser.vue'
  
  export default {
    name: 'App',
    components: { CreateUser },
    data: () => ({
      titulo: "Demo App"
    }),
  };
</script>