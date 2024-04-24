<template>
    <ion-button :color="color" @click="$emit('click')">
      <slot></slot>
    </ion-button>
  </template>
  
  <script lang="ts">
  import { IonButton } from '@ionic/vue';
  import { defineComponent } from 'vue';
  
  export default defineComponent({
    components: { IonButton },
    props: {
      color: {
        type: String,
        default: 'primary',
      },
    },
  });
  </script>
  