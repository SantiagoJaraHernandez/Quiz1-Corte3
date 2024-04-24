<template>
    <ion-fab slot="fixed" vertical="bottom" horizontal="end">
      <ion-fab-button>
        <ion-icon :icon="icon"></ion-icon>
      </ion-fab-button>
      <ion-fab-list side="top">
        <ion-fab-button>
          <ion-icon :icon="document"></ion-icon>
        </ion-fab-button>
        <ion-fab-button>
          <ion-icon :icon="colorPalette"></ion-icon>
        </ion-fab-button>
        <ion-fab-button>
          <ion-icon :icon="globe"></ion-icon>
        </ion-fab-button>
      </ion-fab-list>
    </ion-fab>
  </template>
  
  <script lang="ts">
  import { IonFab, IonFabButton, IonFabList } from '@ionic/vue';
  import { defineComponent } from 'vue';
  import {
    chevronDownCircle,
    document,
    colorPalette,
    globe,
  } from 'ionicons/icons';
  
  export default defineComponent({
    components: { IonFab, IonFabButton, IonFabList },
    setup() {
      return {
        icon: chevronDownCircle,
        document,
        colorPalette,
        globe,
      };
    },
  });
  </script>
  