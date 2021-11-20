<template>
  <ion-app>

    <ion-router-outlet :animated="true" id="sidemenu-content" />
  </ion-app>
</template>


<script lang="ts">
import { defineComponent } from 'vue';

import { 
  IonApp, 
  IonRouterOutlet
} from '@ionic/vue';




export default defineComponent({
  name: 'App',
  components: {
    IonApp,
    IonRouterOutlet,

  }
});
</script>