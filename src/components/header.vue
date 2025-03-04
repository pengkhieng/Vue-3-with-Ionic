<template>
    <IonHeader :translucent="true">
      <IonToolbar>
        <IonButtons slot="start">
          <!-- You can put a back button or a menu button here -->
          <IonButton @click="goBack">
            <IonIcon :icon="arrowBack" />
          </IonButton>
        </IonButtons>
        <IonTitle>{{ title }}</IonTitle>
        <IonButtons slot="end">
          <!-- Optionally add more buttons like settings, logout, etc. -->
          <IonButton @click="openSettings">
            <IonIcon :icon="settingsIcon" />
          </IonButton>
        </IonButtons>
      </IonToolbar>
    </IonHeader>
  </template>
  
  <script>
  import { IonHeader, IonToolbar, IonButtons, IonButton, IonIcon, IonTitle } from '@ionic/vue';
  import { arrowBack, settings } from 'ionicons/icons';
  
  export default {
    name: 'Header',
    props: {
      title: {
        type: String,
        default: 'My App', // Default title
      },
    },
    data() {
      return {
        arrowBack,
        settingsIcon: settings,
      };
    },
    methods: {
      goBack() {
        // Logic to go back to the previous page
        this.$router.go(-1);
      },
      openSettings() {
        // Logic to open settings page or modal
        this.$router.push('/settings');
      },
    },
  };
  </script>
  
  <style scoped>
  /* Optional styling */
  </style>
  