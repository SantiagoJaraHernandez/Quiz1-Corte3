<template>
    <ion-item>
      <ion-label>{{ label }}</ion-label>
      <ion-input :placeholder="placeholder" v-model="value"></ion-input>
    </ion-item>
  </template>
  
  <script lang="ts">
  import { IonItem, IonLabel, IonInput } from '@ionic/vue';
  import { defineComponent, ref } from 'vue';
  
  export default defineComponent({
    components: { IonItem, IonLabel, IonInput },
    props: {
      label: String,
      placeholder: String,
      value: String,
    },
  });
  </script>
  