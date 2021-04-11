<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Ionic-Vue</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content>
      <h1>Dynamic Import Icon</h1>
      <ion-icon :icon="heart"></ion-icon>
      <h1>Global Import Icon</h1>
      <ion-icon icon="heart"></ion-icon>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';
import { heart } from 'ionicons/icons';

export default  {
  name: 'Tab1',
  components: { IonHeader, IonToolbar, IonTitle, IonContent, IonPage },
  setup() {
    return { heart }
  }
}
</script>