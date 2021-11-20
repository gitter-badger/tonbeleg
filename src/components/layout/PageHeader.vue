<template>
  <SideMenu/>
  <ion-header>
    <ion-toolbar>
      <ion-buttons slot="start">
        <ion-menu-button menu="sidemenu"></ion-menu-button>
      </ion-buttons>
      <ion-title>{{ title }}</ion-title>
    </ion-toolbar>
  </ion-header>
</template>


<script lang="ts">
import { defineComponent } from 'vue';

import { 
  IonHeader, IonToolbar, 
  IonButtons, IonMenuButton, IonTitle
} from '@ionic/vue';
import SideMenu from '@/components/layout/SideMenu.vue';

export default defineComponent({
  name: "PageHeader",

  components: {
    IonHeader, IonToolbar, 
    IonButtons, IonMenuButton, IonTitle, SideMenu
  },

  props: {
    title: {
      type: String,
      required: true
    }
  }

});
</script>
