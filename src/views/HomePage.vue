<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Formulario</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true" class="ion-padding">
      <InputGeneric label="Nombre" placeholder="Nombre" v-model="nombre" />
      <InputGeneric label="Fecha Nacimiento" placeholder="Fecha Nacimiento" v-model="fechaNacimiento" />
      <InputGeneric label="Celular" placeholder="Celular" v-model="celular" />
      <InputGeneric label="Correo" placeholder="Correo" v-model="correo" />

      <ButtonGeneric @click="agregar">Agregar</ButtonGeneric>
      <ButtonGeneric @click="modificar">Modificar</ButtonGeneric>
      <ButtonGeneric @click="eliminar">Eliminar</ButtonGeneric>
      <ButtonGeneric @click="consultar">Consultar</ButtonGeneric>

      <FloatingComponent />
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
import InputGeneric from '../components/InputGeneric.vue';
import ButtonGeneric from '../components/ButtonGeneric.vue';
import FloatingComponent from '../components/FloatingComponent.vue';
import { defineComponent, ref } from 'vue';

const nombre = ref('');
const fechaNacimiento = ref('');
const celular = ref('');
const correo = ref('');
const objeto = ref({ key: 'Valor' });

const agregar = () => {
  console.log('Agregado');
};

const modificar = () => {
  console.log('Modificado');
};

const eliminar = () => {
  console.log('Eliminado');
};

const consultar = () => {
  console.log('Consultado');
};
</script>

<style scoped>
</style>
