

<!-- <script setup lang="ts"> -->
<script lang="ts">
   import "./assets/globals.css";
   import Card from "./components/Card.vue";

   export default {
      components: {
         Card
      },
      data() {
         return {
            cidades: [
               {
                  id: 8429,
                  name: "Rio de Janeiro",
                  description: "Ensolarado",
                  icon: "01d",
                  temp: "25",
               },
               {
                  id: 8412,
                  name: "Manaus",
                  description: "Chuvas Fortes",
                  icon: "09d",
                  temp: "25",
               },
               {
                  id: 8454,
                  name: "Brasília",
                  description: "Ensolarado",
                  icon: "10d",
                  temp: "27.4",
               },
            ],
            users: [
               {
                  id: 1,
                  name: "Débora",
                  email: "debora.mc.sammarco@gmail.com"
               },
               {
                  id: 2,
                  name: "Anselmo Sammarco Nunes",
                  email: "noah.kd@gmail.com"
               },
               {
                  id: 3,
                  name: "Noely",
                  email: "noely.gangello@gmail.com"
               },
               {
                  id: 4,
                  name: "Bernardo",
                  email: "bernardo.sammarco.gangello@gmail.com"
               },
            ],
         };
      },
   }
</script>

<template>
   <h1>App Clima</h1>

   <!-- <div class="lista">
      <div class="card" v-for="cidade in cidades" :key="cidade.id">
         <div class="card-img"></div>
         <h3>{{ cidade.name }}</h3>
         <h4>{{ cidade.description }}</h4>
         <div class="temperatura">{{ cidade.temp }}º</div>
      </div> 
   </div> -->
   <section
      style="display: flex; flex-direction: column; gap: 1em;"
   >
      <Card v-for="user in users" :key="user.id" :user="user"/>
   </section>
</template>

<style scoped>
   
</style>