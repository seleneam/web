<template>
    <DataTable />
    <MiBoton />


    <v-row>
      <mi-boton variant="outlined" :etiqueta="etiqueta"></mi-boton>
    </v-row>
    
  </template>
  
  <script setup>
    import { ref } from 'vue';
    //import MiBoton from '@/components/MiBoton.vue';
    import DataTable from '@/components/DataTable.vue';
  
    const etiqueta = ref("CANCELAR");  
    </script>
  