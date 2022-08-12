<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Ionic Vite</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content class="ion-padding">
      <p>
        <ion-button @click="clicked">BUTTON</ion-button>
      </p>
      <ion-card>
        <ion-card-content>
          <!-- <img alt="Vue logo" src="./assets/logo.png" />
          <HelloWorld msg="Hello Vue 3 + TypeScript + Vite" /> -->
        </ion-card-content>
      </ion-card>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import {
  IonContent,
  IonButton,
  IonPage,
  IonHeader,
  IonTitle,
  IonToolbar,
} from "@ionic/vue";
import HelloWorld from "./components/HelloWorld.vue";

export default defineComponent({
  name: "App",
  components: {
    HelloWorld,
    IonHeader,
    IonPage,
    IonButton,
    IonContent,
    IonTitle,
    IonToolbar,
  },
  setup() {
    return {
      clicked: () => alert("clicked"),
    };
  },
});
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
