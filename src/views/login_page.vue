<template>
    <ion-page>
   <ion-header :translucent="true">
        <ion-toolbar>
        <ion-title>Login Page</ion-title>
        </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true" class="ion-padding">
      <!-- <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Login</ion-title>
        </ion-toolbar>
      </ion-header> -->

        
        <div class="login-container">
        <!-- Profile Image -->
        <img :src="logoUrl" alt="Profile Image" class="profile-image" />

        <!-- Login Form -->
        <IonInput v-model="username" placeholder="Username" class="input-field" />
        <IonInput v-model="password" type="password" placeholder="Password" class="input-field" />

        <!-- Login Button -->
        <IonButton expand="full" @click="login">Login</IonButton>
      </div>



      <div id="container">
        <strong class="hello" >chanto muk doch sva.</strong>
      </div>
    </ion-content>
    </ion-page>
</template>

<script setup>
import { ref } from "vue";
import { IonPage, IonContent, IonCard, IonCardContent, IonItem, IonLabel, IonInput, IonButton } from "@ionic/vue";
import router from "@/router";

const username = ref("");
const password = ref("");
const logoUrl = ref("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQsRITgy15ccQD7WyCR7US7T8LxriW-bAmq5A&s");

const login = () => {
  console.log("Username:", username.value);
  console.log("Password:", password.value);
  router.push("/home");
};
</script>

<style scoped>
.login-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 50px;
}

.profile-image {
  width: 80px;
  height: 80px;
  padding: 8px;
  margin-bottom: 20px;
  border: 4px solid greenyellow;
  border-radius: 50%;
}

</style>