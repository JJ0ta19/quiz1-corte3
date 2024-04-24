<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Carrito de compra</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Login</ion-title>
        </ion-toolbar>
      </ion-header>
      <div id="login-container">
        
      
        <div id="description">
          <p>Quiz1-corte3</p>
        </div>
      
        <div id="login-form">
          <InputComponent id="Nombre" name="Nombre" label="Nombre: " />
          <InputComponent type="date" id="Fecha" name="Fecha" label="Fecha de nacimiento: " />
          <InputComponent type="nombre" id="Celular" name="Celular" label="Celular: " />
          <InputComponent type="email" id="correo" name="correo" label="Correo: " />
        </div>

        <p></p>
        <div>
          <ButtonComponent id="save" value="Agregar" fill="outline" color="success"/>  <p></p>
          <ButtonComponent id="update" value="Modificar" fill="outline" color="warning"/>  <p></p>
          <ButtonComponent id="danger" value="Eliminar" fill="outline" color="tertiary"/>  <p></p>
          <ButtonComponent id="dark" value="Consultarr" fill="outline" color="dark"/> 

        </div>
        <div>
          <InputComponent type="password" id="personaId"  />
        </div>

        <!-- <div>
          <ion-button fill="outline">Default</ion-button>
          <ion-button :disabled="true" fill="outline">Disabled</ion-button>
        </div> -->
      </div>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
import ButtonComponent from '@/components/ButtonComponent.vue';
import InputComponent from '@/components/InputComponent.vue';
</script>

<style scoped>
#login-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
}

#cart-image {
  margin-bottom: 20px;
  width: 100px;
}

#description {
  margin-bottom: 20px;
  text-align: center;
}

#description p {
  margin: 0;
  padding: 10px; 
}

#login-form {
  max-width: 300px;
  width: 100%;
}
</style>